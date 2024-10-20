<template>
  <div class="tweet">
    <ProfileImage :image="tweet.user.image" />

    <div class="body">
      <div class="top">
        <span class="user">
          <user :user="tweet.user" />
        </span>

        <Timestamp :timestamp="tweet.timestamp" />
      </div>

      <Message :message="tweet.message"/>

      <Actions />
   
    </div>

    <i class="fas fa-ellipsis-h"></i>


  </div>
</template>

<script setup>

  import {defineProps} from 'vue'
  import ProfileImage from './ProfileImage.vue'
  import User from './User.vue'
  import Timestamp from './Timestamp.vue'
  import Message from './Message.vue'
  import Actions from './Actions.vue'

  defineProps({
    tweet: Object
  })
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
