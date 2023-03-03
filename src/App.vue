<script> 

export default{
  data(){
    return{
      contador:10
    }
  },
  methods: {
    incrementar(){
    this.contador++
  },
  decrementar(){
    if (this.contador > 0) {
        this.contador--
      }
    },
    resetar(){
      this.contador = 0
    }
  }
}

</script> 



<template> 

  <button @click="incrementar">+</button> 
  <button @click="decrementar">-</button>
  <button @click="resetar">C</button> 
  <p>Valor do contador: {{ contador }}</p>
  

</template>



<style scoped> 

button {
  margin-left: 10px;
  background-color: black;
  color: white;
  border:none;
  border-radius: 5px;
  padding: 5px 10px;
  cursor: pointer;
}

</style>