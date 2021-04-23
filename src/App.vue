<template>
  
  <div id="app">
    <cliente :cliente="clienteVictor"/>
    <cliente :cliente="clienteVictor"/>
    <cliente :cliente="clienteVictor"/>
    <cliente :cliente="clienteVictor"/>
    <cliente :cliente="clienteVictor"/>
    
  </div>

</template>

<script>
import cliente from './components/cliente'
//mport produto from './components/produto'
export default {
  name: "App",
  data(){
    return {
      nomeDoVictor: "Paulo V N. Medeiros",
      clienteVictor: {
        nome: "victor Nooblath",
        email: "Victor@gmail.com",
        idade: 99
      }
    }
    
  },
  components: {
    cliente,
    //produto
  }
};
</script>

<style>

</style>
