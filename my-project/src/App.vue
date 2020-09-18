<template>
  <div id="app">
    <div class="header">
      <div class="links">
        <img src="https://raw.githubusercontent.com/Akinoriv/Redsoft-test/5fe5899fab4c6a279e8dba464688de7aea775aa6/my-project/src/assets/Group.svg" class="logo"> 
        <nav>
          <ul class="nav">
            <li>Каталог</li>
            <li>Доставка</li>
            <li>Оплата</li>
            <li>Контакты</li>
            <li>О галерее</li>
          </ul>
        </nav>
      </div>
      <div>
        <input v-model="message" placeholder="Поиск по названию картины">
        <button>Найти</button>
      </div>
    </div>

    <catalog/>

    <div class="footer">
      <div class="links">
        <img src="https://raw.githubusercontent.com/Akinoriv/Redsoft-test/5fe5899fab4c6a279e8dba464688de7aea775aa6/my-project/src/assets/Group.svg" class="logo"> 
        <nav>
          <ul class="nav">
            <li>Каталог</li>
            <li>Доставка</li>
            <li>Оплата</li>
            <li>Контакты</li>
            <li>О галерее</li>
          </ul>
        </nav>
      </div>
      <div>
        <input v-model="message" placeholder="Поиск по названию картины">
        <button>Найти</button>
      </div>
    </div>
  </div>
  
</template>

<script>
import catalog from './components/catalog.vue'

export default {
  name: 'App',
  components: {
    catalog
  }
}
</script>

<style>

img {
  height: 48px;
  width: 48px;
  border: none;
  align-self: center;
}

button {
  /* padding-left: 24px; */
  border: none;
  height: 48px;
  width: 122px;
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

input {
  padding-left: 16px;
  border: 1px solid #E1E1E1;
  box-sizing: border-box;
  height: 48px;
  width: 294px;
  background-color: rgb(246, 243, 243);
  color: #9F9F9F;
  align-self : Inside;
  Font-Family: Merriweather;
  Font-Style: normal;
  Font-Size: 14px;
  Line-Height: 21px;
  Line-Height: 150%;
}

.header {
  padding: 24px;
  /* padding-top: 24px;
  padding-bottom: 24px; */
  background: rgb(246, 243, 243);
  border-bottom: 1px solid #E1E1E1;
  display: flex;
  justify-content: space-between;
  /* width: 100%;
  max-width: 1400px;
  justify-content: space-around;
  position: fixed;
  top: 0px;
  right: 0px;
  left: 0px; */
}


.links {
  display: flex;
  justify-content: space-between;
}

ul{
    padding-left: 24px;
}

.nav {
  display: flex;
  list-style-type: none;
}

  .nav>li {
        margin-left: 24px;
        margin-right: 24px;
        align-self: Center;
        justify-content:start;  
      }

h1 {
  font-weight: bold;
  font-size: 24px;
  /* line-height: 1.7; */
 }

h2 {
  font-weight: normal;
  font-size: 18px;  
 }

h3 {
  font-weight: bold;
  font-size: 16px;
 }

h4 {
  font-weight: bold;
  font-size: 14px;
 }

h5 {
  font-weight: normal;
  font-size: 14px;  
 }

h6 {
  font-weight: 300;
  font-size: 14px;
 }

#app {
  font-family: 'Merriweather', serif;
  color: #343030;
  font-style: normal;
  Font-Size: 14px;
  Line-Height: 21px;
  Line-Height: 150%;
  
  width: 100%;
  padding-right: 15px;
  padding-left: 15px;
  margin-right: auto;
  margin-left: auto;
  max-width: 1258px;

  /* padding: 0 calc(50% - 610px); */
}
</style>
