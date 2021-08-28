<template>
  <h3 id="Title" class="text-left font-weight-thin">
    Inter-Boutique <strong>Digital Market </strong>
    <v-btn id="home-button" depressed color="black" dark @click="goHome"> Home </v-btn>
    <v-container id="products_grid">
      <v-row v-for="i in 2" :key="i" align="center"  style="height: 200px">      
        <v-col v-for="n in 4" :key="n" style="max-width: 225px">
          <clotheCard nombre="Prueba" categoria="Upwear"></clotheCard>
        </v-col>
      </v-row>
    </v-container>

    
    
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

#products_grid {
 position: absolute;
 left: 307px;
}

#home-button{
  position: absolute;
  top: 22px;
  right: -100px;
}
</style>

<script>
import clotheCard from "@/components/clotheCard.vue";

export default {
  name: "Panel",

  components: {
    clotheCard,
  },

  methods:{
    goBack(){
      this.$router.go(-1);
    },
    goHome(){
      this.$router.push('/');
    },

  }
};
</script>