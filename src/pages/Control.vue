<template>
  <v-container fill-height>
    <v-container>
      <v-row>
        <v-col></v-col>
        <v-col class="text-center">
          <v-btn fab x-large>
            <v-icon>keyboard_arrow_up</v-icon>
          </v-btn>
        </v-col>
        <v-col></v-col>
      </v-row>

      <v-row>
        <v-col class="text-right">
          <v-btn fab x-large>
            <v-icon>keyboard_arrow_left</v-icon>
          </v-btn>
        </v-col>
        <v-col class="text-center">
          <v-btn fab x-large>
            <v-icon>pause</v-icon>
          </v-btn>
        </v-col>
        <v-col>
          <v-btn fab x-large class="text-left">
            <v-icon>keyboard_arrow_right</v-icon>
          </v-btn>
        </v-col>
      </v-row>

      <v-row>
        <v-col></v-col>
        <v-col class="text-center">
          <v-btn fab x-large>
            <v-icon>keyboard_arrow_down</v-icon>
          </v-btn>
        </v-col>
        <v-col></v-col>
      </v-row>
    </v-container>
  </v-container>
</template>

<script>
  export default {
    data() {
      return {}
    }
  }
</script>
