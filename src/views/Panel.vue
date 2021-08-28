<template>
  <h3 id="Title" class="text-left font-weight-thin">
    Inter-Boutique <strong>Digital Market </strong>
    <v-row align="center" no-gutters style="height: 50px">
      <v-col v-for="n in 4" :key="n">
        <clotheCard nombre="Prueba" categoria="Upwear"></clotheCard>
      </v-col>
    </v-row>
    
  </h3>
</template>


<style scoped>
#Title {
  position: absolute;
  height: 44px;
  width: 1000px;
  left: 77px;
  top: 50px;

  font-style: normal;
  font-weight: normal;
  font-size: 50px;
  line-height: 74px;
}
</style>

<script>
import clotheCard from "@/components/clotheCard.vue";

export default {
  name: "Panel",

  components: {
    clotheCard,
  }
};
</script>