<script setup>
import Title from "@/components/Title.vue";
</script>

<template>
  <div class="title text-center" style="margin-bottom: 6%;">
    <Title class="logo"/>
    <h1 class="text-center">QLore is a tool for testing servers using simple scripts.</h1>
  </div>
</template>

<style scoped>
.title {
  font-size: 500%;
  user-select: none;
}

.title:hover {
  .logo {
    animation: jump 1s 1;
  }
}

@keyframes jump {
  0% {
    transform: translateY(0);
  }

  50% {
    transform: translateY(-20px);
  }

  100% {
    transform: translateY(0);
  }
}
</style>