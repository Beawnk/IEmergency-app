<template>
    <q-btn class="sec-button">{{text}}</q-btn>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: 'SecondButton',
  props: {text: String},
  data() {  
  }
});

</script>

<style lang="scss">
.sec-button {
    border-radius: 100px;
    height: 80px;
    width: 300px;
    font-size: 30px !important;
    text-transform: initial;
    color: $primary;
    border: 3px solid $primary;
}

</style>