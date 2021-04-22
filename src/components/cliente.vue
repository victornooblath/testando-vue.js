<template>
    <div id="cliente">
        
        <input type="text" v-model="nome">
        <hr>
        <input type="text" v-model="descricao">
        <h2 id='cliente-nome'>{{ nome }}</h2>
        <p>Descrição do Cliente - {{ descricao }}</p>
        {{2+2*4}}
    </div>
    
    

</template>

<script> 
export default {
    data() {
        return {
            nome: "vic",
            numero: "",
            email: "",
            idade: 0,
            descricao: "lorem ipsum",
        }
    }
}
</script>

<style scoped>
    #cliente {
        color:rgb(52, 52, 61);
        background-color:rgba(126, 195, 208, 0.885);
        max-width: 600px;
        height: 200px;
        
    }

    #cliente-nome {
        color: rgb(94, 16, 133);
    }
</style>