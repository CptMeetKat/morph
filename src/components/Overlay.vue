<template>
  <div>
    <v-overlay v-model="overlay" content-class="overlay">
      <template #activator="{ isActive, props }">
        <v-btn v-bind="props">
          Overlay is {{ isActive ? 'open' : 'closed' }}
        </v-btn>
      </template>
      <v-card>
        <v-card-title class="text-h5">Overlay Content</v-card-title>
        <v-card-text>This is the content inside the overlay.</v-card-text>
      </v-card>
    </v-overlay>
  </div>
</template>


<style>
.overlay
{
  margin: auto;
  position: relative;
}
</style>

<script>
export default {
  data() {
    return {
      overlay: true
    };
  }
};
</script>
