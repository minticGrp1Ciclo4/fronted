<template>
<div>
  <v-sheet class="rounded" color="grey lighten-1"  elevation="1" height="150" width="200">
        <v-row  align="end" style="height: 170px;">
          <v-col align="end" >
            <v-chip>{{nombre}}</v-chip>      
            <span style="width: 25px">  </span>
            <v-chip>{{categoria}}</v-chip>
          </v-col>
        </v-row>
      </v-sheet>
</div>
  
</template>

<script>
export default {
  name: "clotheCard",
  props:['nombre','categoria']
    
  
  
};
</script>