<template>
    <div :class="{'cliente': !isPremium, 'cliente-premium': isPremium}">
        <h4>Nome : {{cliente.nome}} </h4>
        <hr>
        <p>Email : {{cliente.email}}</p>
        <p v-if="showIdade == true">Idade : {{cliente.idade}}</p>
        <p v-else>O usuário optou por esconder a idade</p>
        
    </div>
    
    

</template>

<script> 
export default {
    data() {
        return {
            isPremium: false
        }
    },
    props: {
        cliente: Object,
        showIdade: Boolean
    }
}
</script>

<style scoped>
    .cliente {
        background-color: #bbb1ae;
        max-width: 600px;
        height: 180px;
        padding: 1%;
        margin-top: 2%;
        
    }
    .cliente-premium{
        background-color: #000000;
        color: yellow;
        max-width: 600px;
        height: 180px;
        padding: 1%;
        margin-top: 2%;
    }

    #cliente-nome {
        color: rgb(94, 16, 133);
    }
</style>