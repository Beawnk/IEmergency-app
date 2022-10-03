<template>
  <div class="header-text">
    <h1>{{ text1 }}</h1>
    <h2>{{ text2 }}</h2>
    <div class="emergency-text">
      <p>{{ text3 }}</p>
      <q-btn flat round color="primary">
        <img src="../assets/warning.png" />
      </q-btn>

      <a href=""> </a>
    </div>
  </div>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  data() {
    return {
      text1: "Olá, ####!",
      text2: "O que você quer denunciar?",
      text3: "Em caso de emergências, clique no botão vermelho ao lado.",
    };
  },
});
</script>

<style lang="scss">
.header-text {
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
    margin-right: 30px;
  }
  .emergency-text {
    display: flex;
    align-items: center;
    justify-content: space-between;
    button {
      width: 50px;
      height: 50px;
      margin-top: 20px;
      img {
        height: 40px;
      }
    }
  }
}
</style>
