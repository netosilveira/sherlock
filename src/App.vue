<template>
  <v-app id="inspire">
    <v-navigation-drawer v-model="drawer"  app>
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title class="text-h6"> Application </v-list-item-title>
          <v-list-item-subtitle> subtext </v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>

      <v-divider></v-divider>

      <v-list dense nav>
        <v-list-item v-for="item in items" :key="item.title" link>
          <v-list-item-icon>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar app :color="'#000000'" height="140px">
      <v-app-bar-nav-icon
        @click="drawer = !drawer"
        style="color:white;background-color:grey"
      ></v-app-bar-nav-icon>
      <div class="main-menu">
        <img src="https://i.imgur.com/pYRXWdz.png" height="120%" />
      </div>
    </v-app-bar>

    <v-main>
      <router-view></router-view>
    </v-main>
  </v-app>
</template>

<script>
export default {
  data: () => ({ drawer: false }),
};
</script>

<style>
.main-menu {
  height: 100%;
  width: 100%;
  display: flex;
  justify-content: center;
}
</style>
