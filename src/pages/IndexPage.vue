<template>
  <ul class="complaint-list">
    <li class="complaints">
      <h4>Aglomeração durante a pandemia</h4>
      <img src="..//assets/coronavirus.png" />
    </li>
    <li class="complaints">
      <h4>Violência doméstica</h4>
      <img src="..//assets/danger.png" />
    </li>
    <li class="complaints">
      <h4>Aglomeração durante a pandemia</h4>
      <img src="..//assets/danger.png" />
    </li>
    <li class="complaints">
      <h4>Incêndio</h4>
      <img src="..//assets/danger.png" />
    </li>
    <li class="complaints">
      <h4>Aglomeração durante a pandemia</h4>
      <img src="..//assets/danger.png" />
    </li>
    <li class="complaints">
      <h4>Aglomeração durante a pandemia</h4>
      <img src="..//assets/danger.png" />
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
    justify-content: flex-end;
    padding: 10px;

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
