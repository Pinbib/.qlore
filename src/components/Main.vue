<script>
import Button from "@/components/Button.vue";

export default {
  components: {Button},
  props: {
    load: Function
  }
};
</script>

<template>
  <div class="row">
    <div class="col-md-3"></div>
    <Button class="btnInstall col-md-2" title="Window"
            url="https://github.com/Pinbib/QLore/raw/main/PKG/win/QLore.exe" @click="load()"/>
    <Button class="btnInstall col-md-2" title="MacOS"
            url="https://github.com/Pinbib/QLore/raw/main/PKG/macos/QLore" @click="load()"/>
    <Button class="btnInstall col-md-2" title="Linux"
            url="https://github.com/Pinbib/QLore/raw/main/PKG/linux/QLore" @click="load()"/>
    <div class="col-md-3"></div>
  </div>
  <div class="row" style="margin-top: 3%;">
    <div class="col-md-4"></div>
    <Button class="btnInstall col-md-2" title="VSCode"
            url="https://github.com/Pinbib/QLore/raw/main/VSCode/QLoreVSCode.zip" @click="load()"/>
    <Button class="btnInstall col-md-2" title="GitHub" url="https://github.com/Pinbib/QLore"/>
  </div>
  <div class="row" style="margin-top: 3%;">
    <div class="col-md-5"></div>
    <Button class="btnInstall col-md-2" title="Docs"
            url="https://github.com/Pinbib/QLore/?tab=readme-ov-file#qlore"/>
  </div>
</template>

<style scoped>
.btnInstall {
  margin: 2px;
  text-align: center;
  border: solid #9e9e9e 3px;
  border-radius: 6px;
  user-select: none;
}

.btnInstall:hover {
  cursor: pointer;
  box-shadow: 0 0 0 2px #9e9e9e;
  transform: scale(1.05);
}
</style>