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

<style lang="scss" scoped>
@import "../style/variables";
.comics {
    width: calc(100% / 6);
    margin-top: 40px;
    img {
        height: 150px;
        width: 150px;
    }
        a {
            text-decoration: none;
        }
            & h6:hover,
            & img:hover {
                color: $mainColor;
            }
}
h6 {
    max-width: 150px;
    text-transform: uppercase;
    margin: 10px 0;
    color: white;
}
</style>