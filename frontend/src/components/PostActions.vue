<script setup>
import TheIcon from './TheIcon.vue';
0;
</script>

<template>
  <div class="postActions">
    <TheIcon icon="like" fill="none" stroke="#000000"> </TheIcon
    ><span>1w</span>
    <TheIcon icon="comment" fill="none" stroke="#000000"> </TheIcon
    ><span>1w</span>
    <TheIcon icon="favorite" fill="none" stroke="#000000"> </TheIcon
    ><span>99w</span>
  </div>
</template>

<style scoped>
.postActions {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  justify-items: center;
  justify-self: end;
  column-gap: 16px;
  row-gap: 4px;
}

.postActions > svg {
  width: 32px;
  height: 32px;
  grid-row: 1 / 2;
  cursor: pointer;
}
</style>
