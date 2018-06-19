<template>
  <div class="counter">
    <h1 class="counter__title">{{ number }}</h1>
    <button class="counter__button" type="button" @click="increment">Increment</button>
    <button class="counter__button" type="button" @click="decrement">Decrement</button>
  </div>
</template>

<script>
  export default {
    data(){
      return{
        number: 0,
      }
    },
    methods:{
      increment(){
        if(this.number >= 0){
          this.number++
        }
      },
      decrement(){
        if(this.number > 0){
          this.number --
        }
      }
    }
  }
</script>

<style scoped>

  .counter {
    display: inline-block;
    margin-left: 30%;
  }

  .counter__title {
    text-align: center;
  }

  .counter__button {
    display: inline-block;
    padding: 20px;
    margin: 10px;
    font-weight: 700;
    border-radius: 5px;
    box-shadow: 0px 0px 5px 0px rgb(11, 11, 114);
  }


</style>
