<template>
  <div>
      <h1>Bem Vindo a Tela Pedidos</h1>
      <button id="teste" @click="IrParaTelaMenuPrincipal">IrParaTelaMenuPrincipal</button>
      <button id="teste1" @click="IrParaTelaCardapio">IrParaTelaCardápio</button>
  </div>
</template>

<script>
export default {
data:function(){
    return{

    }
}, methods:{
    IrParaTelaMenuPrincipal:function(){
    this.$router.push('/')
  }, IrParaTelaCardapio:function(){
    this.$router.push('/ViewTelaCardapio')
  }
}
}
</script>

<style>
#body,html{
    background-color: rgb(64, 186, 131);
}

#teste{
  border: 2px solid black;
  color: red;
  background-color: black ;
}

#teste1{
  border: 2px solid white;
  color: white;
  background-color: green;
  cursor: pointer;
}
</style>