<script>
export default {
  data() {
    return {
      image: "vue.svg",
    };
  },
  methods: {
    getImageUrl(name) {
      return new URL("../assets/${name}", import.meta.url).href;
    },
  },
};
</script>
<template>
  <img :src="getImageUrl(image)" alt="" />
  <img src="/vite.svg" alt="" />
</template>

<style></style>
