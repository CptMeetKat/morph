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

    <main>
      <div style="min-width: 500px; max-width:675px; margin: auto;">
        <ProjectReel />
        <ProjectReel />
      </div>
    </main>
  </v-app>
</template>


<style scope>
</style>
