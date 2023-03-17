
<script>
export default {
  data:() => ({
    contador:0,
  }),

  methods: {
    incrementar() 
    {
    this.contador++;
    },

    disminuir()
    {
      this.contador--;
    },

    reset()
    {
      this.contador = 0;
    },

  },


};


</script>

<template>
  <div class="container">
    <h2>VUE 3</h2>
    <img src="./assets/logo.svg" alt="" width="150" height="150">
    <hr>
    <h2>Contador {{contador}}</h2>
    <button @click="incrementar">+1</button>
    <button @click="disminuir">-1</button>
    <button @click="reset">Reset</button>
  </div>
  

</template>


<style>

  .container{
    text-align: center;
  }

  button{
    font-size: 20px;
    padding: 10px;
    margin: 5px;
  }

  h2{
    color: white;
  }
</style>
