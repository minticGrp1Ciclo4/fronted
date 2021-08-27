<template>
  <v-container>
    <h1 id="Title" class="text-left .font-weight-thin">Inter-Boutique</h1>
    <v-btn id="s-button" depressed color="black" dark @click="toPanel"> Revisar Stock </v-btn>
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
</style>
<script>
export default {
  name: "Home",

  methods:{
    toPanel(){
      this.$router.push('/Panel')
    }
  }

};
</script>
