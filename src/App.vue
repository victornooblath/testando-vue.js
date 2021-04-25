<template>
  
  <div id="app">
    

    <div v-for="(cliente,index) in clientes" :key="cliente.id">
      <h4>{{ index + 1 }}</h4>
      <cliente :cliente="cliente"/>
      <h4>Edição: </h4>
      <input type="text" v-model="cliente.nome">
      <input type="text" v-model="cliente.email">
      <hr>

    </div>

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
      },
      clientes: [
        {
          id: 22,
          nome: "Carlos André",
          email: "Carlos@gmail.com",
          idade: 49
        },
        {
          id:45,
          nome: "Pedro vasconselos",
          email: "pedro@gmail.com",
          idade: 19
        },
        {
          id: 46,
          nome: "joão vasconselos",
          email: "joão@gmail.com",
          idade: 19
        }
      ]
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
