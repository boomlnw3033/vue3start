<script setup>
import { ref } from "vue";

const like = ref(0);
const sad = ref(0);

function likeClick() {
  like.value++;
}
function sadClick() {
  sad.value++;
}
</script>

<template>
  <div class="like_sad">
    <button @click="likeClick()" class="b1">
      Like <i class="bi bi-heart-fill"></i> {{ like }}
    </button>
    <button @click="sadClick()" class="b2">
      Sad <i class="bi bi-hand-thumbs-down"></i> {{ sad }}
    </button>
  </div>
</template>

<style scoped>
.like_sad{
  display: flex;
  justify-content: space-between;
  margin-bottom: 10px;
  gap: 20px;
}
.b1{
  background-color: aqua
}
.b2{
  background-color: rgb(229, 108, 108)
}
</style>
