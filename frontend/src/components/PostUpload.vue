<script setup>
import TheIcon from './TheIcon.vue';
import TheButton from './TheButton.vue';
</script>

<template>
  <Teleport to="body">
    <div class="modal">
      <div class="backdrop"></div>
      <div class="modalContent">
        <button class="closeBtn"><TheIcon icon="close" /></button>
        <div class="postUpload">
          <label class="upload">
            <TheIcon icon="upload-image" />
            <input type="file" accept="image/*" class="fileChooser" />
          </label>
          <div class="postContent">
            <textarea
              placeholder="寫下你的想法..."
              class="postContentInput"
            ></textarea>
            <TheButton class="pubBtn">發布</TheButton>
          </div>
        </div>
      </div>
    </div>
  </Teleport>
</template>

<style scoped>
.modal {
  position: fixed;
  width: 100vw;
  height: 100vh;
  max-width: 100%;
  left: 0;
  top: 0;
  display: grid;
  place-items: center;
}

.backdrop {
  background: rgba(0, 0, 0, 0.56);
  position: absolute;
  width: 100%;
  height: 100%;
  left: 0;
  top: 0;
}

.modalContent {
  position: relative;
  background: white;
  border-radius: 52px;
  overflow: hidden;
}

.closeBtn {
  position: absolute;
  background: none;
  border: none;
  right: 14px;
  top: 10px;
}

.closeBtn svg {
  width: 54px;
  height: 54px;
}

.postUpload {
  width: 50vw;
  height: 70vh;
  display: grid;
  grid-template-rows: 4fr 1fr;
}

.preview {
  width: 100%;
  height: 100%;
  object-fit: cover;
  min-height: 0;
}
.upload {
  display: grid;
  place-items: center;
  cursor: pointer;
  min-height: 0;
}
.upload > svg {
  width: 254px;
  height: 316px;
}

.fileChooser {
  opacity: 0;
  position: absolute;
}

.postContent {
  display: grid;
}
.postContentInput {
  border-bottom: none;
  resize: none;
  padding: 12px 24px;
}

.postContentInput::placeholder {
  color: #757575;
}

.pubBtn {
  align-self: end;
  justify-self: end;
  position: relative;
  right: 24px;
  bottom: 18px;
}
</style>
