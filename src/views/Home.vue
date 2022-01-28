<template>
  <div>
    <div class="parallax" />

    <div class="container">
      <div class="box">
        <img src="https://i.imgur.com/YbVgWOz.jpg" />
        <span>CSS</span>
      </div>
      <div class="box">
        <img src="https://i.imgur.com/FbuPx7H.jpg" />
        <span>Image</span>
      </div>
      <div class="box">
        <img src="https://i.imgur.com/zaq7mpb.jpg" />
        <span>Hover</span>
      </div>
    </div>
    <!-->
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
    <-->
  </div>
</template>

<style>
.container {
  display: flex;
  width: 100%;
  padding: 4% 2%;
  box-sizing: border-box;
  height: 100vh;
  background-color:black;
}

.box {
  flex: 1;
  overflow: hidden;
  transition: .5s;
  margin: 0 2%;
  box-shadow: 0 20px 30px rgba(0,0,0,.1);
  line-height: 0;
}

.box > img {
  width: 200%;
  height: calc(100% - 10vh);
  object-fit: cover; 
  transition: .5s;
}

.box > span {
  font-size: 3.8vh;
  display: block;
  text-align: center;
  height: 10vh;
  line-height: 2.6;
}

.box:hover { flex: 1 1 50%; }
.box:hover > img {
  width: 100%;
  height: 100%;
}
 

.parallax {
  background-image: url("https://i.imgur.com/YJsdazN.jpeg");

  min-height: 800px;

  /* Create the parallax scrolling effect */
  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
</style>
<script>
export default {
  data() {
    return {
      items: [
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
