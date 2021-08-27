<template>
    <div >
       <v-img
            id="img1"
            class="white--text "
            max-height="150"
            max-width="250"
            src="@/assets/Camiseta.png"
          >
            <v-container >
              <v-layout >
                <v-flex >
                  <h5 class="text-right "><br>Camisetas</h5>
                  <h5 class="text-right font-weight-thin">Encuentra tu estilo</h5>
                </v-flex>
              </v-layout>
            </v-container>
          </v-img>
    
    
        
    </div>
</template>



<script>
export default {
  name: "thumbnailCard",
  props: ['imagen'],
  data(){
    return{
      imagesrc: this.imagen
    }
    
  }
  
};
</script>