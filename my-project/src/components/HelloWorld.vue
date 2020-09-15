<template>
  <div class="header">
    <img src="https://github.com/Akinoriv/Redsoft-test/blob/master/my-project/src/assets/Group.png?raw=true" class="logo"> 
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

</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.header {
  display: flex;
  width: 100%;
  justify-content: space-between;
  max-width: 1180px;
  margin: 0 auto;
  align-self: center;
  box-sizing: border-box;
  padding-left: 50px;
  padding-right: 50px;
}

.nav {
  justify-content: flex-start;
  display: flex;
  list-style-type: none;
}

.nav>li {
  margin-left: 15px;
}

.logo {
  display: block;
  width: 58;
  height: 100;
  background-image: url()
}

h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
