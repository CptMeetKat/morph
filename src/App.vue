<script setup>
import ProjectReel from './components/ProjectReel.vue'
</script>

<template>
  <v-app>
    <header>
      <v-container>
        <v-app-bar scroll-behavior="hide" scroll-threshold="1">
        <template v-slot:prepend>
            <!-- <v-app-bar-nav-icon></v-app-bar-nav-icon> -->
          </template>

          <v-app-bar-title>Morph</v-app-bar-title>
        </v-app-bar>
      </v-container>
    </header>

    <main class="reel hidden-scroll">
      <div style="min-width: 412; max-width:675px; margin: auto;">
        <ProjectReel class="reel-item" />
        <ProjectReel class="reel-item" />
        <ProjectReel class="reel-item" />
        <ProjectReel class="reel-item" />
      </div>
    </main>
  </v-app>
</template>


<style scoped>

.reel
{
  max-height: 100vh;
  overflow-y: scroll;
  scroll-snap-type: y mandatory;

  -ms-overflow-style: none;  /* IE and Edge */
  scrollbar-width: none;  /* Firefox */
}

/* Hide scrollbar for Chrome, Safari and Opera */
.reel-scroll::-webkit-scrollbar {
    display: none;
}

.reel-item
{
  scroll-snap-align: start;
}

</style>
