<template>
  <div class="welcome-container">
    <div class="name-wrap">
      <img src="../assets/Logo.png" />
      <h1>IEmergency</h1>
    </div>
    <h1>Bem vindo</h1>
  </div>
  <div class="login-wrap">
    <a href="/">Esqueceu a senha?</a>
    <MainButton text="Cadastre-se" :to="{ path: '/index', hash: '/' }"/>
    <SecondButton text="Login" style="margin-bottom: 2rem;" :to="{ path: '/index', hash: '/' }"/>
  </div>
</template>


<script>
import { defineComponent } from "vue";
import MainButton from "src/components/MainButton.vue";
import SecondButton from "../components/SecondButton.vue";

export default defineComponent({
    name: "LoginPage",
    components: { MainButton, SecondButton }
});

</script>

<style lang="scss">
.welcome-container {
  background: $main-gradient;
  border-radius: 0px 0px 50px 50px;
  padding: 100px 0px 25px 0px;
  h1 {
    font-size: 40px;
    font-weight: 300;
    color: white;
    text-align: center;
    line-height: 50px;
  }
  .name-wrap {
    display: flex;
    flex-direction: column;
    align-items: center;
    h1 {
      font-weight: 500;
      color: $title-color;
      padding-bottom: 3rem;
      text-shadow: 0px 6px 8px #26262669;
    }
    img {
      width: 150px;
      border-radius: 40px;
      box-shadow: 0px 10px 20px #26262669;
    }
  }
}
.login-wrap {
  display: flex;
  flex-direction: column-reverse;
  align-items: center;
  justify-content: center;
  padding-top: 60px;
  a {
    text-decoration: none;
    color: #6d14c0b6;
    font-size: 15px;
    margin-top: 1rem;
  }
}

</style>
