<template>
  <main>
      <section class="section_up">
          <div class="container">
              <h1> &ndash; &ndash; &gt; Content goes here &lt;&ndash; &ndash; </h1>
          </div>
      </section>
      <section class="section_down">
            <div class="container">
            
            </div>
        </section>
      
  </main>
</template>

<script>
export default {
    name : "Main",
}
</script>

<style scoped>
    .section_up {
        height: 120px;
        background-color: black;
    }
    .container {
        max-width: 70%;
        margin: auto;
    }
    h1 {
        line-height: 120px;
        color: white;
        font-size: 30px;
    }
    .section_down {
        height: 150px;
        background-color: #2482F9;
    }
</style>