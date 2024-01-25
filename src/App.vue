<script>
import Header from "@/components/Header.vue";
import Main from "@/components/Main.vue";
import Loading from "@/components/Loading.vue";

(async () => {
  let version = await fetch("https://raw.githubusercontent.com/Pinbib/QLore/main/package.json");
  version = await version.json();
  document.getElementById("version").innerHTML = "v" + version.version;
})();

export default {
  components: {Loading, Main, Header},
  methods: {
    load() {
      document.querySelector(".l").style.display = "block";
      setTimeout(() => document.querySelector(".l").style.display = "none", 2000);
    }
  }
};
</script>

<template>
  <div class="container-fluid">
    <span id="version" class="d-inline-flex">vError</span>
    <Header style="margin-top: 5%"/>
    <br>
    <Main :load="load"/>

    <Loading class="l"/>
  </div>
</template>
<style scoped>
.l {
  display: none;
}
</style>