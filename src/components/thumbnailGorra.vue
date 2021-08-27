<template>
    <div >
       <v-img
            id="img1"
            class="white--text "
            max-height="137"
            max-width="250"
            src="@/assets/Gorra.png"
          >
            <v-container >
              <v-layout >
                <v-flex >
                  <h5 class="text-right"><br> Accesorios</h5>
                  <h5 class="text-right font-weight-thin">Define tu outfit</h5>
                </v-flex>
              </v-layout>
            </v-container>
          </v-img>
    
    
        
    </div>
</template>

<style scoped>

</style>

<script>
export default {
  name: "thumbnailGorra",
  props: ['imagen'],
  data(){
    return{
      imagesrc: this.imagen
    }
    
  }
  
};
</script>