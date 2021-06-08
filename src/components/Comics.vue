<template>
  <div class="comics">
      <img :src="cover.thumb" :alt="cover.series">
      <h6>{{ cover.series }}</h6>
  </div>
</template>

<script>
export default {
    name: "Comics",
    props: ["cover"]
}
</script>

<style scoped>
.comics {
    width: calc(100% / 6);
    margin-top: 30px;
}
.comics img {
    height: 120px;
    width: 120px;
    }
h6 {
    max-width: 120px;
    text-transform: uppercase;
    margin: 10px 0;
    color: white;
}
</style>