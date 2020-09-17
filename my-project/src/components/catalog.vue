<template>

  <div class="page">
    <div class="title">
      <h1>Картины эпохи Возрождения</h1>
    </div>
    <div class="wrap">
      <div class="paintings">

        <div class="paintings-item">
          <img src="" alt="">
          <h2> «Рождение Венеры» <br> Сандро Боттичелли </h2>
          <h6> 2 000 000 $ </h6>
          <h3> 1 000 000 $ </h3>
          <button> Купить </button>
        </div>

        <div class="paintings-item">
          <img src="" alt="">
          <h2> «Тайная вечеря» <br> Леонардо да Винчи </h2>
          <h6></h6>
          <h3> 3 000 000 $ </h3>
          <button> Купить </button>
        </div>

        <div class="paintings-item">
          <img src="" alt="">
          <h2> «Сотворение Адама» <br> Микеланджело </h2>
          <h6></h6>
          <h3> 5 000 000 $ </h3>
          <button> В корзине </button>
        </div>

        <div class="paintings-item">
          <img src="" alt="">
          <h2> «Урок анатомии» <br> Рембрандт </h2>
          <h6></h6>
          <h3> Продана на аукционе </h3>
        </div>

      </div>
      
    </div>
      
  </div>

</template>

<script>
export default {
  name: 'catalog',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.page {
  padding-top: 39px;
  padding-bottom: 320px;
}

.title {

  /* max-width: 1400px; */
  /* padding-left: 7%; */
  justify-content: start;
  /* position: fixed; */
}

.wrap {
  padding:24px;
  margin: 0 auto;
  width: 100%;
  max-width: 1400px;
  display: flex;
  /* max-width: 1200px; */

  justify-content: space-around;
}

.paintings {
  display: grid;
  grid-template: 25% 25% 25% 25%;
  justify-self: center;
}
.paintings-item {
  height: 328px;
  width: 280px;
  /* position: absolute; */
  /* left: 0%;
  right: 0%;
  top: 0%;
  bottom: 0%; */

  border: 1px solid #E1E1E1;
  box-sizing: border-box;
}


</style>
