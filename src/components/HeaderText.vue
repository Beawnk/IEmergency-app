<template>
  <div class="header-text">
    <h1>{{text1}}</h1>
    <h2>{{text2}}</h2>
    <p>{{text3}}</p>

  </div>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  data() {
    return {
      text1: 'Olá, ####!',
      text2: 'O que você quer denunciar?',
      text3: 'Em caso de emergências, clique no botão vermelho acima.'
    }
  }
})
</script>

<style lang="scss">
  .header-text{
    /* background: $primary; */
    margin-left: 1rem;
    color: #fff;
    h1 {
      font-size: 35px;
      margin-top: 4rem;
      line-height: 10px;
      font-weight: 500;
    }
    h2 {
     font-size: 19px;
     font-weight: 400;
    }
    p {
     margin-top: 2rem;
     font-size: 14px;
     max-width: 80%;
    }
  }
</style>