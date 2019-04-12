<template>
  <v-app>
    <v-toolbar>
      <v-toolbar-title>
       Vue Check List
      </v-toolbar-title>
    </v-toolbar>
    <v-container>
      <v-layout row justify-center>
        <v-card class="ma-5" width="600">
          <Item v-for="item in items" v-bind:text="item" />
        </v-card>
      </v-layout>
    </v-container>
  </v-app>
</template>

<script>
import Item from './components/Item'

export default {
  name: 'App',
  components: {
    Item
  },
  data () {
    return {
      items: [
        "Make pancakes",
        "Get Amos insulin",
        "Read a book",
        "Take a nap"
      ]
    }
  }
}
</script>
