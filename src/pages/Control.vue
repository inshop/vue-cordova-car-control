<template>
  <v-container fill-height>
    <v-container>
      <v-row>
        <v-col></v-col>
        <v-col class="text-center">
          <v-btn fab x-large @click="forward">
            <v-icon>keyboard_arrow_up</v-icon>
          </v-btn>
        </v-col>
        <v-col></v-col>
      </v-row>

      <v-row>
        <v-col class="text-right" @click="left">
          <v-btn fab x-large>
            <v-icon>keyboard_arrow_left</v-icon>
          </v-btn>
        </v-col>
        <v-col class="text-center">
          <v-btn fab x-large @click="stop">
            <v-icon>pause</v-icon>
          </v-btn>
        </v-col>
        <v-col>
          <v-btn fab x-large class="text-left" @click="right">
            <v-icon>keyboard_arrow_right</v-icon>
          </v-btn>
        </v-col>
      </v-row>

      <v-row>
        <v-col></v-col>
        <v-col class="text-center">
          <v-btn fab x-large @click="back">
            <v-icon>keyboard_arrow_down</v-icon>
          </v-btn>
        </v-col>
        <v-col></v-col>
      </v-row>
    </v-container>
  </v-container>
</template>

<script>
  import bluetoothSerial from '../../src-cordova/node_modules/cordova-plugin-bluetooth-serial/www/bluetoothSerial'

  export default {
    methods: {
      forward() {
        bluetoothSerial.write('f;')
      },
      back() {
        bluetoothSerial.write('b;')
      },
      left() {
        bluetoothSerial.write('l;')
      },
      right() {
        bluetoothSerial.write('r;')
      },
      stop() {
        bluetoothSerial.write('s;')
      }
    }
  }
</script>
