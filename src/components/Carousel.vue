<template>
  <v-carousel
    :show-arrows="false"
    :height="'92.8vh'"
    cycle
    hide-delimiters
    :progress="true"
  >
    <v-carousel-item v-for="(item, i) in items" :key="i">
      <v-img :src="item.src" :max-height="'90%'" :max-width="'100%'"></v-img>
    </v-carousel-item>
  </v-carousel>
</template>


<script>
export default {
  data() {
    return {
      items: [
        {
          src: "https://i.imgur.com/HuY290W.jpg",
        },
        {
          src: "https://i.imgur.com/YbVgWOz.jpg",
        },
        {
          src: "https://i.imgur.com/FbuPx7H.jpg",
        },
        {
          src: "https://i.imgur.com/zaq7mpb.jpg",
        },
      ],
    };
  },
};

</script>