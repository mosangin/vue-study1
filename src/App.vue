<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <div>
    <h4>{{product[0]}}</h4>
    <p>{{price1}}</p>
  </div>
  <div>
    <h4>{{product[1]}}</h4>
    <p>{{priceRandom}}</p>
  </div>
  <div>
    <h4>{{product[2]}}</h4>
    <p>{{priceRandom}}</p>
  </div>
</template>

<script>

export default {
  name: 'App',
  data(){
    return {
      product : ['역삼동원룸','수원원룸','강남원룸'],
      price1 : 60,
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
  color: #2c3e50;
  margin-top: 60px;
}
</style>
