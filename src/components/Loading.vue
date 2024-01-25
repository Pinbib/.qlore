<script setup>
import Load from "@/components/Icons/Load.vue";
</script>

<template>
  <div>
    <div class="overlay text-center">
      <div class="content">
        <Load class="loadSvg"/>
        <br>
        <span>Loading<span id="points"></span></span>
      </div>
    </div>
  </div>
</template>

<style scoped>
.loadSvg {
  animation: spin 2s infinite;
}

#points {
  display: inline-block;
  width: 15px;
}

.overlay {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 9999;
}

.content {
  background-color: #141414;
  padding: 25px;
  border-radius: 5px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.3);
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