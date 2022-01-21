<template>
  <v-app>
    <Header />
    <v-main>
      <Copia />
    </v-main>
  </v-app>
</template>

<script>
import Header from "./components/Header";
import Copia from "./components/Copia";

export default {
  name: "App",

  components: {
    Header,
    Copia,
  },

  data: () => ({
    //
  }),
};
</script>
