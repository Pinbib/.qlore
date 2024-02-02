<script>
export default {
  props: {title: String, url: String}
};
</script>

<template>
  <a :href="url" class="link-light">{{ title }}</a>
</template>

<style scoped>
a {
  text-decoration: none;
}
</style>