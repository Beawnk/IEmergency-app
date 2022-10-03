<template>
  <q-btn push class="complaints">
    <h4>{{text}}</h4>
    <img :src="require(`../assets/${imgUrl}`)" />
  </q-btn>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: 'ComplaintsCard',
  props: {text: String, imgUrl: String},
  data() {  
  }
});

</script>

<style lang="scss">
  .complaints {
    margin: 10px;
    width: 180px;
    height: 130px;
    background-color: white;
    border-radius: 20px;
    padding: 10px;
    box-shadow: 0px 1px 10px 2px #00000014;
    &::before{
      display: none;
    }
    > span {
      display: flex;
      flex-direction: column-reverse;
      justify-content: space-around;
      align-items: flex-start;
      img {
        width: 50px;
        opacity: 50%;
      }
      h4 {
        font-size: 12px;
        line-height: 16px;
        color: #767676;
        text-transform: initial;
        text-align: left;
      }
    }
  }
</style>
