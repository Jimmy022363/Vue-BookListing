<template>
  <v-app>
    <v-toolbar app>
      <v-toolbar-title class="headline text-uppercase">
        <span>Vuetify</span>
        <span class="font-weight-light">MATERIAL DESIGN</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn
        flat
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
      >
        <span class="mr-2">Latest Release</span>
      </v-btn>
    </v-toolbar>

    <v-content>
      <img src="./assets/logo.png">
      <BookList/>
    </v-content>

  </v-app>
</template>

<script>

import BookList from './components/BookList'
//import BookList from './components/BookList/BookList'
//import HelloWorld from './components/HelloWorld'
//import BookForm from './components/BookForm'
//import BookList2 from './components/BookList2'

export default {
  name: 'App',
  components: {
    BookList,
  },
  data () {
    return {
      //
    }
  }
}
</script>
