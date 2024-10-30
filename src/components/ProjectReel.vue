<script setup>
</script>

<template>
      <div class="reel-card" >
        <div>
          <v-carousel :cycle=true height="500px"> <!-- height is on here -->
            <v-carousel-item
              src="https://fastly.picsum.photos/id/907/500/500.jpg?hmac=1JG7-2YxQq4FkxYTIwNTsXH1FJw5WZoGoXCTCONnoJw"
              cover
            ></v-carousel-item>

            <v-carousel-item
              src="https://fastly.picsum.photos/id/128/1080/566.jpg?hmac=WdBcuFwIPlWtFn1Xh5KfObTiai0-vfZB7CWDU__8m2o"
              cover
            ></v-carousel-item>

            <v-carousel-item
              src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
              cover
            ></v-carousel-item>
          </v-carousel>
        </div>

        <div class="reel-summary">
          <div> <b> JAVA, Spring boot, APIs </b> </div>
          <div> Created a weather forecasting app in Java that integrates with public APIs to display real-time weather data and seven-day forecasts, featuring a clean, intuitive GUI built with JavaFX. </div>
        </div>
      </div>
</template>

<style scoped>
.reel-summary {
  padding: 1em;
}

.reel-card
{
  align-content: center;
  height:100vh;
}
</style>
