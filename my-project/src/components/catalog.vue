<template>

  <div class="page">
    <div class="page__title">
      <h1> Картины эпохи Возрождения </h1>
    </div>

    <div class="wrap">
      <div class="paintings">

        <div class="painting__item">
          <img class="painting__item-img" 
            src="https://github.com/Akinoriv/Redsoft-test/blob/master/my-project/src/assets/painting-63186_1280%201.png?raw=true" 
            alt="«Рождение Венеры»"
          >
          <h2 class="painting__item-name"> «Рождение Венеры» <br> Сандро Боттичелли </h2>
          <div class="painting__item-block">
            <div class="painting__price-box">
              <h6 class="painting__price-discount"> 2 000 000 $ </h6>
              <h3 class="painting__price--new"> 1 000 000 $ </h3>
            </div>
            <div class="painting__button-box">
              <button class="painting__button"> Купить </button>
            </div>
          </div>
        </div>

        <div class="painting__item">
          <img class="painting__item-img"
            src="https://github.com/Akinoriv/Redsoft-test/blob/master/my-project/src/assets/ae973f6678e037cd297053384aa7dca0%201.png?raw=true"
            alt="«Тайная вечеря»"
          >
          <h2 class="painting__item-name"> «Тайная вечеря» <br> Леонардо да Винчи </h2>
          <div class="painting__item-block">
            <div class="painting__price-box">
              <h3 class="painting__price"> 3 000 000 $ </h3>
            </div>
            <div class="painting__button-box">
              <button class="painting__button"> Купить </button>
            </div>
        </div>
        </div>

        <div class="painting__item">
          <img class="painting__item-img" 
            src="https://github.com/Akinoriv/Redsoft-test/blob/master/my-project/src/assets/image-19%201.png?raw=trues" 
            alt="«Сотворение Адама»"
          >
          <h2 class="painting__item-name"> «Сотворение Адама» <br> Микеланджело </h2>
          <div class="painting__item-block">
            <div class="painting__price-box">
              <h6 class="painting__price-discount"> 6 000 000 $ </h6>
              <h3 class="painting__price--new"> 5 000 000 $ </h3>
            </div>

            <div class="painting__button-box">
              <!-- <h2 v-if="seen">SEEN</h2> -->
              <button  v-if="seen" class="painting__button"  v-on:click="toggleSeen"  >{{ button.text }}</button>

              <button  v-else id="hide-seen" class="painting__button painting__button--basket" v-on:click="toggleSeen"> 
                <img class="foter__contacts-img" 
                src="https://github.com/Akinoriv/Redsoft-test/blob/master/my-project/src/assets/phone.png?raw=true"> 
                {{ button.text }} </button>
            </div>

            <!-- <div id="example-1" class="painting__button-box">
              <button v-on:click="counter += true" class="painting__button painting__button--basket"> {{counter}} </button>
            </div> -->
          </div>
        </div>

        <div class="painting__item painting__item--sold">
          <img class="painting__item-img" 
            src="https://github.com/Akinoriv/Redsoft-test/blob/master/my-project/src/assets/20152310142330%201.png?raw=true" 
            alt="«Урок анатомии»"
          >
          <h2 class="painting__item-name"> «Урок анатомии» <br> Рембрандт </h2>
          <div class="painting__item-block--sold">
            <h3 class="painting__price"> Продана на аукционе </h3>
          </div>
        </div>
      </div>
    </div>
  </div>

</template>

<script>
export default {

  data() {

    return {
         button: {
      text: 'Купить'
    },
      seen: true
    }
  },

  methods: {  
  

    toggleSeen: function() {
      this.seen = !this.seen;
      this.button.text = this.seen ? 'Купить' : 'В корзине';
    },

    buttonClick: function() {
      if(this.show) {
        return 'Скрыть'
      }
      return 'Показать'
    },

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">

.page {
  /* min-height: calc(100vh - 80px); */
  padding-top: 102px;
  padding-bottom: 96px;
  // box-sizing: border-box;
	// min-height: 100%; 
}

.page__title {

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

.painting__item {
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

.painting__item-name {
  padding-left: 24px;
  text-align: left;
  line-height: 1.5;
}

.painting__item-img  {
  height: 158px;
  width: 280px;
}

.painting__item-block {
  margin:  24px;
  /* padding-top: ; */
  display: flex;
  align-items: flex-end;
  justify-content: space-between;
}

.painting__price-box {
  align-self: center;
}

.painting__price {
  margin: 0;
  text-align: start;
} 

.painting__price--new {
  margin: 0;
  text-align: start;
}

.painting__price-discount {
  color: #A0A0A0;
  text-decoration: line-through;
  margin: 0;
  text-align: start;
}

.painting__item--sold {
  background :rgb(246, 243, 243);
  opacity:.4; 
}

.painting__item-block--sold {
  margin: 24px;
  text-align: left;
  display: flex;
  align-items: flex-end;
}

.painting__button {
   /* padding-left: 24px; */
  border: none;
  height: 48px;
  width: 120px;
  background-color: #382E2B;
  color: #F4F6F9;
  Font-Family: Merriweather;
  Font-Style: Bold;
  Font-Size: 14px;
  Line-Height: 21px;
  Line-Height: 150%;
  /* justify-content: space-evenly; */
  justify-content:right;
}

.painting__button--basket {
  background-color: #5B3A32
  
}


</style>
