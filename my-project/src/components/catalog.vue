<template>

  <div class="page">
    <div class="title">
      <h1>Картины эпохи Возрождения</h1>
    </div>
    <div class="wrap">
      <div class="paintings">

        <div class="paintings-item">
          <img src="https://github.com/Akinoriv/Redsoft-test/blob/master/my-project/src/assets/painting-63186_1280%201.png?raw=true" 
                                                                                                              alt="«Рождение Венеры»">
          <h2> «Рождение Венеры» <br> Сандро Боттичелли </h2>
          <div class="paintings-item__block">
            <div class="paintings-item__price">
              <h6> 2 000 000 $ </h6>
              <h3> 1 000 000 $ </h3>
            </div>
            <div class="paintings-item__button">
              <button> Купить </button>
            </div>
          </div>
        </div>

        <div class="paintings-item">
          <img src="https://github.com/Akinoriv/Redsoft-test/blob/master/my-project/src/assets/ae973f6678e037cd297053384aa7dca0%201.png?raw=true" alt="«Тайная вечеря»">
          <h2> «Тайная вечеря» <br> Леонардо да Винчи </h2>
          <div class="paintings-item__block">
            <div class="paintings-item__price">
              <h3> 3 000 000 $ </h3>
            </div>
            <div class="paintings-item__button">
              <button> Купить </button>
            </div>
        </div>
        </div>

        <div class="paintings-item">
          <img src="https://github.com/Akinoriv/Redsoft-test/blob/master/my-project/src/assets/image-19%201.png?raw=trues" alt="«Сотворение Адама»">
          <h2> «Сотворение Адама» <br> Микеланджело </h2>
          <div class="paintings-item__block">
            <div class="paintings-item__price">
              <h6> 6 000 000 $ </h6>
              <h3> 5 000 000 $ </h3>
            </div>
            <div class="paintings-item__button">
              <button> В корзине </button>
            </div>
          </div>
        </div>

        <div class="paintings-item sold">
          <img src="https://github.com/Akinoriv/Redsoft-test/blob/master/my-project/src/assets/20152310142330%201.png?raw=true" alt="«Урок анатомии»">
          <h2> «Урок анатомии» <br> Рембрандт </h2>
          <div class="sold__item">
            <h3> Продана на аукционе </h3>
          </div>
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
  padding-top: 14px;
  padding-bottom: 320px;
}

.title {

  /* max-width: 1400px; */
  /* padding-left: 7%; */
  justify-content: start;
  padding: 24px;
  padding-bottom: 14px;
  /* position: fixed; */
}

.wrap {
  /* padding:24px; */
  margin: 0 auto;
  width: 100%;
  max-width: 1400px;
  display: flex;
  justify-content: space-around;

  /* justify-content: space-between; */
}

/* .paintings {
} */

.paintings-item {
  height: 328px;
  width: 282px;
  float:left; 
  text-align:center;
  margin: 14px;
  /* position: absolute; */
  /* left: 0%;
  right: 0%;
  top: 0%;
  bottom: 0%; */
  border: 1px solid #E1E1E1;
  box-sizing: border-box;
}

.paintings-item>h2 {
  padding-left: 24px;
  text-align: left;
  line-height: 1.5;
}

.paintings-item>img {
  height: 158px;
  width: 280px;
}

.paintings-item__block{
  margin:  24px;
  /* padding-top: ; */
  display: flex;
  align-items: flex-end;
  justify-content: space-between;
}

.paintings-item__price {
  align-self: center;

}
.paintings-item__price>h3 {
  text-decoration: line-through;
  margin: 0;
  text-align: start;
}

.paintings-item__price>h6 {
  color: #A0A0A0;
  text-decoration: line-through;
  margin: 0;
  text-align: start;
}

.sold {
  background :rgb(246, 243, 243); opacity:.4;
}

.sold__item {
  margin: 24px;
  text-align: left;
  display: flex;
  align-items: flex-end;

}

</style>
