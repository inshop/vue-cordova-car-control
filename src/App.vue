<template>
  <v-app>
    <router-view/>

    <v-bottom-navigation
        absolute
        grow
        color="primary"
    >
      <v-btn x-large :to="{ name: 'Control'}">
        <span>Car control</span>
        <v-icon>directions_car</v-icon>
      </v-btn>

      <v-btn x-large :to="{ name: 'Bluetooth'}">
        <span>Bluetooth</span>
        <v-icon>bluetooth</v-icon>
      </v-btn>

      <v-btn x-large :to="{ name: 'Settings'}">
        <span>Settings</span>
        <v-icon>settings</v-icon>
      </v-btn>
    </v-bottom-navigation>
  </v-app>
</template>

<script>
  export default {
    name: 'App',
  }
</script>
