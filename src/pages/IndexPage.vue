<template>
  <ul class="complaint-list">
    <ComplaintsCard text="Aglomeração durante a pandemia" imgUrl="coronavirus.png" />
    <ComplaintsCard text="Violência doméstica" imgUrl="femenine.png" />
    <ComplaintsCard text="Acidente de trânsito" imgUrl="accident.png" />
    <ComplaintsCard text="Incêndio" imgUrl="danger.png" />
    <ComplaintsCard text="Assalto" imgUrl="robber.png" />
    <ComplaintsCard text="Árvore caída" imgUrl="disaster.png" />
  </ul>
</template>
<script>

import { defineComponent } from "vue";
import ComplaintsCard from 'components/ComplaintsCard.vue'

export default defineComponent({
  name: "IndexPage",

  components: {
    ComplaintsCard,
  },
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
}
</style>
