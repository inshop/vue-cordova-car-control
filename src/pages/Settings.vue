<template>
  <v-container fill-height>
    <v-container>
      <v-row>
        <v-col>
          <h2 class="mb-5">Car back lights</h2>

          <v-switch v-model="backLights" :label="switchLabel" inset></v-switch>
        </v-col>
      </v-row>

      <v-row>
        <v-col>
          <h2 class="mb-5">Car back lights</h2>

          <v-slider
              v-model="frontLights"
              prepend-icon="highlight"
          ></v-slider>
        </v-col>
      </v-row>
    </v-container>
  </v-container>
</template>

<script>
  export default {
    data() {
      return {
        backLights: true,
        frontLights: 30,
      }
    },
    computed: {
      switchLabel() {
        return 'Car back lights ' + (this.backLights ? 'on' : 'off')
      }
    }
  }
</script>
