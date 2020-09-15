<template>
  <div id="app">
    <HelloWorld/>
    <div class="header">
      <img src="https://raw.githubusercontent.com/Akinoriv/Redsoft-test/5fe5899fab4c6a279e8dba464688de7aea775aa6/my-project/src/assets/Group.svg" class="logo"> 
      <nav>
        <ul class="nav">
          <li>Каталог</li>
          <li>Доставка</li>
          <li>Оплата</li>
          <li>Контакты</li>
          <li>О галерее</li>
          <input v-model="message" placeholder="Поиск по названию картины">
          <button>Найти</button>
        </ul>
      </nav>
    </div>
  </div>
  
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
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
  border: none;
  height: 48px;
  width: 112px;
  background-color: #382E2B;
  color: #F4F6F9;
  Font-Family: Merriweather;
  Font-Style: Bold;
  Font-Size: 14px;
  Line-Height: 21px;
  Line-Height: 150%;
  align-self: Center;
  
  justify-content:right;
}

input {
  border: none;
  height: 48px;
  width: 416px;
  background-color: #E1E1E1;
  color: #9F9F9F;
  align-self : Inside;
  Font-Family: Merriweather;
  Font-Style: Regular;
  Font-Size: 14px;
  Line-Height: 21px;
  Line-Height: 150%;
  justify-content:right; 
  margin-left: 150px; 

}

.header {
  display: flex;
  width: 100%;
  max-width: 1338.5px;
  margin: 0 auto;
  
}

.nav {
  display: flex;
  list-style-type: none;
}
  .nav>li {
        margin-left: 24px;
        margin-right: 24px;
        justify-content:start;  
        align-self: Center; 
      }

#app {
  font-family: 'Merriweather', serif;
  color: #343030;
  Font-Style: Regular;
  Font-Size: 14px;
  Line-Height: 21px;
  Line-Height: 150%;
  background:#E5E5E5;
  Fill: Solid
}
</style>
