<template>
  <v-app>
    <Header />
    <v-main>
      <HelloWorld />
    </v-main>
  </v-app>
</template>

<script>
import Header from "./components/header/Header";
import HelloWorld from "./components/hello-world/HelloWorld";

export default {
  name: "App",

  components: {
    Header,
    HelloWorld,
  },

  data: () => ({
    //
  }),
};
</script>
