<template>
  <div id="app">

       <h2 id="cliente-title">  Clientes </h2>
    <h3> INFORMAÇÕES SOBRE OS CLIENTES </h3>

   
         
         

    <br><br>
      <Cliente/>
      <br><br>
      <Cliente/>
      <br><br>
      <Cliente/>
      <br><br>
      
      
      
    
  </div>
</template>

<script>


import Cliente from './components/Cliente';

export default {
  name: 'App',
    data(){
      return{

      

          nome:"",
          profissao:"",
          endereco:"",
          email:"",
          indicacao:""
          

      }

      
    },
        
      components: {

      Cliente

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
