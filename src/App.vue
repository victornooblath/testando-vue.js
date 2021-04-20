<template>
  
  <div id="app">
    <hr>
      <h4>Lista de produtos!</h4>
    <hr>
    <produto/>
    <produto/>

    <h1>
      Guia Clientes
      <cliente/>
      <cliente/>
      <cliente/>
      <cliente/>
    </h1>
    
  </div>

</template>

<script>
import cliente from './components/cliente'
import produto from './components/produto'
export default {
  name: "App",
  components: {
    cliente,
    produto
  }
};
</script>

<style>

</style>
