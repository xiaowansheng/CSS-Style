<script setup lang="ts">
defineOptions({
  name: 'FullScreenLoading'
})
const loading = ref(true)
</script>

<template>
  <div class="page-loading" v-show="loading">
    <span class="loading"></span>
  </div>
</template>

<style lang="scss" scoped>
.page-loading {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(135, 209, 224, 0.6);
  /* opacity: 0; */
  transition: opacity 0.3s;
  z-index: 999;
}

.page-loading .loading {
  position: absolute;
  top: calc(50% - 50px);
  left: calc(50% - 50px);
  transform: translate(-50%, -50%);
  width: 100px;
  height: 100px;
  background: #81ecec;
  perspective: 120px;
  /* transition: background .2s; */
  animation: pageLoading 1.8s infinite ease-in-out;
}

@keyframes pageLoading {
  0% {
    transform: perspective(120px) rotateX(0deg) rotateY(0deg);
    background: #55efc4;
  }

  50% {
    transform: rotateY(0deg) rotateX(-180.1deg);
    background: #74b9ff;
  }

  100% {
    transform: rotateY(-179.9deg) rotateX(-180deg);
    background: #00cec9;
  }
}
</style>
