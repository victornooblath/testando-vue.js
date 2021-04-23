<template>
  
  <div id="app">
    <cliente :cliente="clienteVictor" :showIdade="true"/>
    <cliente :cliente="clienteVictor" :showIdade="true"/>
    <cliente :cliente="clienteVictor" :showIdade="true" />
    <cliente :cliente="clienteVictor" :showIdade="false"/>
    <cliente :cliente="clienteVictor" :showIdade="true"/>
    
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
        idade: 89
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
