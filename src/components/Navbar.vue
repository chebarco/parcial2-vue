<template>
  <v-app-bar app color="white" flat>
    <v-badge color="white" dot>
      <v-img src="../assets/logo.paogi.png" contain width="100"></v-img>
    </v-badge>



    <v-spacer></v-spacer>
    <v-badge color="black" overlap content="3" class="mr-2 mt-1">
      <v-avatar color="grey" size="40">
        <v-icon x-small color="black">fas fa-shopping-cart</v-icon>
      </v-avatar>
    </v-badge>
  
  </v-app-bar>
</template>

<script>
export default {};
</script>

<style>
.v-toolbar__title {
  font-size: 1rem !important;
}
</style>