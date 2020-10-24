<template>
  <div id="app">
    <div class="row justify-content-around">

      <Conversor nome_moeda1="Euro" nome_moeda2="Real " valor_moeda1="1" valor_moeda2="6.67"/>
      <Conversor nome_moeda1="Euro" nome_moeda2="Dolar" valor_moeda1="1" valor_moeda2="1.19"/>
      <Conversor nome_moeda1="Dolar" nome_moeda2="Real" valor_moeda1="1" valor_moeda2="5.62"/>
      <Conversor nome_moeda1="Yen" nome_moeda2="Real" valor_moeda1="1" valor_moeda2="0.054"/>
      <Conversor nome_moeda1="Euro" nome_moeda2="Yen" valor_moeda1="1" valor_moeda2="124.21"/>
    </div>
    <div class="row  justify-content-around">
          <Conversor nome_moeda1="Real" nome_moeda2="Euro " valor_moeda1="1" valor_moeda2="0.15"/>
          <Conversor nome_moeda1="Dolar" nome_moeda2="Euro" valor_moeda1="1" valor_moeda2="0.84"/>
          <Conversor nome_moeda1="Real" nome_moeda2="Dolar" valor_moeda1="1" valor_moeda2="0.18"/>
          <Conversor nome_moeda1="Real" nome_moeda2="Yen" valor_moeda1="1" valor_moeda2="18.64"/>
          <Conversor nome_moeda1="Yen" nome_moeda2="Euro" valor_moeda1="1" valor_moeda2="0.081"/>
    </div>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Conversor from './components/Conversor.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld,
    Conversor
  }
}
</script>

<style>
#app {

}
</style>
