<template>
  <v-app>
    <Navbar />
    <v-container fluid>
      <v-row>
        <v-col cols="12">
          <v-card class="mx-auto rounded-xl" flat>
            <v-img
              src="../assets/INICIObanner.jpg"
              max-height="100%"
              max-width="100%"
              contain
            >
            </v-img>
          </v-card>
          <v-card-title class="top ml-10">
            <h2 class="title1">Vivi tu momento soñado!</h2>
          </v-card-title>
          <v-card-text class="ml-10">
            <v-row>
              <v-col cols="4">
                <v-text-field
                  label="Busca tu producto Paogi"
                  class="d-none d-sm-none d-md-flex"
                  filled
                  prepend-inner-icon="mdi-magnify"
                  rounded
                  outlined
                >
                </v-text-field>
              </v-col>
              <v-col cols="2" class="marginLeft">
                <v-btn
                  color="black"
                  rounded
                  dark
                  x-large
                  class="py-7 d-none d-sm-none d-md-flex"
                  >Buscar</v-btn
                >
              </v-col>
            </v-row>
          </v-card-text>

          <v-toolbar flat color="transparent" class="mt-5">
            <v-toolbar-title class="text-h6"
              >Nuestros Productos</v-toolbar-title
            >
            <v-spacer></v-spacer>
          </v-toolbar>
          <Product />

            <v-toolbar flat color="" class="mb-4">
              <v-toolbar-title class="popu">Populares</v-toolbar-title>
              <v-spacer></v-spacer>
            </v-toolbar>
            <Pack />
        </v-col>
      </v-row>
    </v-container>
    <Footer />
  </v-app>
</template>

<script>
import Navbar from "../components/Navbar";
import Footer from "../components/Footer";
import Product from "../components/Product.vue";
import Pack from "../components/Pack.vue";

export default {
  name: "Home",
  data: () => ({
    toggle_exclusive: 1,
  }),
  components: {
    Navbar,
    Footer,
    Product,
    Pack,
  },
};
</script>
<style >
.popu{
  margin-left: 80px;
  font-size: 50px !important;
  margin-top: 200px !important;
  color: pink;
  
}
.marginLeft {

  margin-left: -90px;
}
.mtop {
  margin-top: 100px;
}
.mbottom {
  margin-bottom: 100px;
}
.v-card.borderme {
  border: 2px solid black !important;
}
.v-card.borderout {
  border: 1px solid grey !important;
}
.v-btn:not(.v-btn--round).v-size--default.add {
  min-width: 0px !important;
}
.theme--light.v-sheet--outlined.mobile {
  border: 2px solid black !important;
}
@media only screen and (max-width: 600px) {
  h2.title1 {
    font-size: 15px;
  }
  h2.title2 {
    font-size: 15px;
  }
  .top {
    margin-top: 20px;
  }
}
@media only screen and (min-width: 600px) {
  .top {
    margin-top: 70px;
  }
}
@media only screen and (min-width: 768px) {
  .top {
    margin-top: 120px;
  }
}
</style>
