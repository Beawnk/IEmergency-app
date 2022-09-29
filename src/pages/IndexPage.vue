<template>
  <ul class="complaint-list">
    <li class="complaints">
      <h4>Aglomeração durante a pandemia</h4>
      <img src="..//assets/coronavirus.png" />
    </li>
    <li class="complaints">
      <h4>Violência doméstica</h4>
      <img src="..//assets/femenine.png" />
    </li>
    <li class="complaints">
      <h4>Acidente de trânsito</h4>
      <img src="..//assets/accident.png" />
    </li>
    <li class="complaints">
      <h4>Incêndio</h4>
      <img src="..//assets/danger.png" />
    </li>
    <li class="complaints">
      <h4>Assalto</h4>
      <img src="..//assets/robber.png" />
    </li>
    <li class="complaints">
      <h4>Árvore caída</h4>
      <img src="..//assets/disaster.png" />
    </li>
  </ul>
</template>
<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "IndexPage",
});
</script>

<style lang="scss">
.complaint-list {
  padding: 0px;
  height: 85%;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  flex-direction: column;
  align-items: center;

  .complaints {
    margin: 10px;
    width: 180px;
    height: 130px;
    background-color: white;
    border-radius: 20px;
    display: flex;
    flex-direction: column-reverse;
    justify-content: space-around;
    padding: 10px;
    box-shadow: 0px 1px 10px 2px #00000014;

    img {
      width: 50px;
      opacity: 50%;
    }
    h4 {
      font-size: 12px;
      line-height: 16px;
      color: #767676;
    }
  }
}
</style>
