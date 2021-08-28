<template>
  <v-sheet color="grey lighten-4" elevation="1" height="150" width="200">
      <v-container >
              <v-layout>
                <v-flex>  
                  <v-row align="end" no-gutters >                  
                  <v-chip class="font-weight-thin" color="grey lighten-1">{{nombre}}</v-chip>
                  <v-chip class="font-weight-thin" color="grey lighten-1">{{categoria}}</v-chip>
                  </v-row>
                </v-flex>
              </v-layout>
            </v-container>
  </v-sheet>
</template>

<script>
export default {
  name: "clotheCard",
  props:['nombre','categoria'],
  data(){
    return{
    }
    
  }
  
};
</script>