<template>
  <div class="comics">
      <a href="#">
        <img :src="cover.thumb" :alt="cover.series">
      </a>
      <a href="#">
        <h6>{{ cover.series }}</h6>
      </a>
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
    height: 150px;
    width: 150px;
}
.comics h6:hover,
.comics img:hover {
    color: #2179E5;
}
h6 {
    max-width: 150px;
    text-transform: uppercase;
    margin: 10px 0;
    color: white;
}
.comics a {
    text-decoration: none;
}
</style>