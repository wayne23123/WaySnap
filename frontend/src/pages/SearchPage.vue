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
    <h1 class="title">搜尋結果: test</h1>

    <PostList>
      <PostItem v-for="n in 10"></PostItem>
    </PostList>

    <!-- <PostDetails /> -->
    <!-- <PostUpload /> -->
  </div>
</template>

<style scoped>
.title {
  font-weight: 600;
  font-size: 24px;
  margin-bottom: 44px;
}
</style>
