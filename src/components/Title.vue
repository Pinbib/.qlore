<script setup>
import Q from "@/components/Icons/Q.vue";
</script>

<template>
  <div>
    <Q class="Q"/>
    Lore
  </div>
</template>

<style scoped>
div:hover > .Q {
  animation: spin 2s 1;
}

@keyframes spin {
  from {
    transform: rotateZ(0deg);
  }

  to {
    transform: rotateZ(-360deg);
  }
}
</style>