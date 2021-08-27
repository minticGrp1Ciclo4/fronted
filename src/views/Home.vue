<template>
  <v-container>
    <h1 id="Title" class="text-left .font-weight-thin">Inter-Boutique</h1>
    <v-btn id="s-button" depressed color="black" dark @click="toPanel">
      Revisar Stock
    </v-btn>
    <thumbnail-card id="thumb-1" imagen="@/assets/Camiseta.png"></thumbnail-card>
    <thumbnailGorra id="thumb-2"></thumbnailGorra>
    <thumbnailSweater id="thumb-3"></thumbnailSweater>
  </v-container>
</template>



<style scoped>
#Title {
  position: absolute;
  width: 612px;
  height: 94px;
  left: 77px;
  top: 172px;

  font-style: normal;
  font-weight: normal;
  font-size: 72px;
  line-height: 74px;
}

#s-button {
  font-size: 12px;
  font-style: normal;
  font-weight: normal;
  text-align: center;
  top: 294px;
  right: 12px;
}
#thumb-1 {
  position: absolute;
  width: 400px;
  height: 25px;
  left: 400px;
  top: 473px;
}

#thumb-2 {
  position: absolute;
  width: 400px;
  height: 20px;
  left: 700px;
  top: 473px;
}

#thumb-3 {
  position: absolute;
  width: 400px;
  height: 20px;
  left: 1000px;
  top: 473px;
}
</style>
<script>
import thumbnailCard from "@/components/thumbnailCard.vue";
import thumbnailGorra from "@/components/thumbnailGorra.vue";
import thumbnailSweater from "@/components/thumbnailSweater.vue";
export default {
  name: "Home",

  components: {
    thumbnailCard,
    thumbnailGorra,
    thumbnailSweater
    
  },

  methods: {
    toPanel() {
      this.$router.push("/Panel");
    },
  },
};
</script>
