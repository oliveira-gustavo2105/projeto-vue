<template>
    
    
    <div :class="{'cliente': plus, 'cliente-plus': !plus }">
    
    

        
        <input type="text" v-model="nome" placeholder="Nome">
         <input type="text" v-model="profissao" placeholder="Profissão">
         <input type="text" v-model="endereco" placeholder="Local de Trabalho">
         <input type="email" v-model="email" placeholder="E-mail">
         <input type="text" v-model="indicacao" placeholder="Indicação">

         <button @click="trocaPlus">Plus</button>
         
         
        
        <h2>Nome: {{nome}} </h2>
     
     <hr>
        <h2>Profissão: {{profissao}}</h2>
        
        <hr>
           
        <h2>Empresa: {{endereco}}</h2>
        
        <hr>
                       
        <h2>E-mail: {{email}}</h2>
        <hr>
                    
        <h2>Indicação: {{indicacao}}</h2>
        <hr>
        <br> <br>

        

    </div>
    
    
        


   
</template>

<script>
export default {
    data(){
        return{

            nome: "",
            profissao: "",
            endereco: "",
            email: "",
            indicacao: "",
            plus:Boolean,
            
        }
    },
    methods: {
        trocaPlus: function(){

            this.plus = !this.plus;
        }


    }
  
  
  }
</script>

<style scoped>

    .cliente{
        color: purple;
        background-color: #f0fff0;
        

    }

   

    .cliente-plus{

        color: blueviolet;
        background-color: navajowhite;

    }


</style>>

