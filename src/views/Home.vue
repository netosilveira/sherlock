<template>
  <div class="home">
    <v-carousel :show-arrows="false" :height="700">
      <v-carousel-item
        v-for="(item, i) in items"
        :key="i"
        :src="item.src"
        
      ></v-carousel-item>
    </v-carousel>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          src: 'https://pps.whatsapp.net/v/t61.24694-24/187639660_2170477436438250_3759099548713262802_n.jpg?ccb=11-4&oh=01_AVweMm-hPyfu3rKooQeiR8-Pp6bXcPAdUrv4xpFLpU2GjQ&oe=61F76640'
        },
        { src: 'https://pps.whatsapp.net/v/t61.24694-24/187639660_2170477436438250_3759099548713262802_n.jpg?ccb=11-4&oh=01_AVweMm-hPyfu3rKooQeiR8-Pp6bXcPAdUrv4xpFLpU2GjQ&oe=61F76640'},
        { src: 'https://pps.whatsapp.net/v/t61.24694-24/187639660_2170477436438250_3759099548713262802_n.jpg?ccb=11-4&oh=01_AVweMm-hPyfu3rKooQeiR8-Pp6bXcPAdUrv4xpFLpU2GjQ&oe=61F76640'},
        { src: 'https://pps.whatsapp.net/v/t61.24694-24/187639660_2170477436438250_3759099548713262802_n.jpg?ccb=11-4&oh=01_AVweMm-hPyfu3rKooQeiR8-Pp6bXcPAdUrv4xpFLpU2GjQ&oe=61F76640'},
        { src:'https://pps.whatsapp.net/v/t61.24694-24/187639660_2170477436438250_3759099548713262802_n.jpg?ccb=11-4&oh=01_AVweMm-hPyfu3rKooQeiR8-Pp6bXcPAdUrv4xpFLpU2GjQ&oe=61F76640'}
      ]
    }
  }
}
</script>
