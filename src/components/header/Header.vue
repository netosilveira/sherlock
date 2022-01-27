<template>
  <v-app class="teste">
    <v-toolbar dark color="grey" class="teste">
      <v-toolbar-title>
        <img
          src="https://sherlockjuices.com/img/sherlock.png"
          alt="Sherlock"
          height="30px"
        />
      </v-toolbar-title>
      <v-toolbar-item>
        <v-btn flat> Teste 1 </v-btn>
        <v-btn flat> Teste 2 </v-btn>
        <v-btn flat> Teste 3 </v-btn>
      </v-toolbar-item>
    </v-toolbar>
  </v-app>
</template>

<script>
export default {
  setup() {},
};
</script>
<style scoped>
.teste {
  height: 40px;
}
</style>
