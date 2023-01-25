<template>
  <div style="background-color: azure">
    <div class="app">
      <div class="sidebar"><SideBarLeft></SideBarLeft></div>
      <div>
        <div v-for="n in 5" :key="n" class="likesad" style="margin: 2rem">
          <div><BlockMeme></BlockMeme></div>
        </div>
      </div>
      <div class="sidebar"><SideBarRight></SideBarRight></div>
    </div>
  </div>

  <!-- <div v-for="n in 5" :key="n">{{ n }}<LikeSad></LikeSad></div> -->
</template>

<script setup>
import SideBarLeft from "./components/SideBarLeft.vue";
import SideBarRight from "./components/SideBarRight.vue";
import BlockMeme from "./components/BlockMeme.vue";
</script>

<style scoped>
.block-meme {
  background-color: azure;
  opacity: 0.3;
}
p {
  color: #000;
}
.app {
  display: flex;
  justify-content: space-between;
  gap: 20px;
}
.likesad {
  padding-left: 2rem;
}
.sidebar {
  padding: 2rem;
  background-color: aliceblue;
}
</style>
