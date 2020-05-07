<template>
  <div id="app">
      <button id="teste" @click="IrParaTelaCardapio">IrParaTelaCardapio</button>
      <button id="teste1" @click="IrParaTelaPedidos">IrParaTelaPedidos</button>
      <button id="botãoLogin" @click="IrParaTelaLogin">Login</button>
      <button id="botãoCadastro" @click="IrParaTelaCadastro">Cadastrar-se</button>
  </div>
</template>

<script>
export default {
data:function(){
  return{

  }
}, methods:{
   IrParaTelaCardapio:function(){
     this.$router.push("/ViewTelaCardapio")
   },  IrParaTelaPedidos:function(){
       this.$router.push("/ViewTelaPedidos")
     }, IrParaTelaLogin:function(){
       this.$router.push("/ViewTelaLogin")
     }, IrParaTelaCadastro:function(){
       this.$router.push("/ViewTelaCadastro")
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
  background-color: black;
  cursor: pointer;
}

#teste1{
  border: 2px solid white;
  color: white;
  background-color: green;
  cursor: pointer;
}

#botãoLogin{
  border: 2px solid black;
  color: blue;
  background-color: white;
  cursor: pointer;
}
</style>