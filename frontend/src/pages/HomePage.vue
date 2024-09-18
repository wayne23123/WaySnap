<script setup>
import TheIcon from '../components/TheIcon.vue';
import TheAvatar from '../components/TheAvatar.vue';
import PostDetails from '../components/PostDetails.vue';
import PostActions from '../components/PostActions.vue';
import PostUpload from '../components/PostUpload.vue';
import PostList from '../components/PostList.vue';
import PostItem from '../components/PostItem.vue';
</script>

<template>
  <div>
    <PostList>
      <PostItem v-for="n in 10"></PostItem>
    </PostList>

    <!-- <PostDetails /> -->
    <PostUpload />
  </div>
</template>
