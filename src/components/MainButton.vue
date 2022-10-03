<template>
    <q-btn class="main-button">{{text}}</q-btn>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: 'MainButton',
  props: {text: String},
  data() {  
  }
});

</script>

<style lang="scss">
.main-button {
    border-radius: 100px;
    height: 80px;
    width: 300px;
    font-size: 30px !important;
    text-transform: initial;
    color: white !important;
    background-color: $primary;
    border: 3px solid $primary;
}

</style>
