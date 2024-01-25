<script>
export default {
  props: {title: String, url: String}
};
</script>

<template>
  <div><a :href="url" class="link-light">{{ title }}</a></div>
</template>

<style scoped>
a {
  text-decoration: none;
}
</style>