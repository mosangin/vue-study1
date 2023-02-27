<template>

  <div class="menu">
    <a v-for="(a,i) in menu1" :key="i">{{a}}</a>    
  </div>
  <div v-for="(a,i) in product" :key="i">
    <h4>{{product[i]}}</h4>
    <p v-for="(priceList,i) in price1" :key="i">{{priceList}}</p>
  </div>
</template>

<script>

export default {
  name: 'App',
  data(){
    return {
      menu1 : ['Home','Products','About'],
      product : ['역삼동원룸','수원원룸','강남원룸'],
      price1 : [60, 80, 90],
      priceRandom : '가격은아무거나',
    }
  },
  components: {
   
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
.menu{
  background: #2c3e50;
  padding: 15px;
  border-radius: 5px;
}
.menu a{
  color: #fff;
  padding: 10px;
}
</style>
