<template>
  <v-app dark id="app">
    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
    <v-footer
      :absolute="!fixed"
      app
      class="justify-center"
    >
      <span>&copy; {{ new Date().getFullYear() }}, Made with <span style="color:red">&#x2764;</span> in Montreal</span>
    </v-footer>
  </v-app>
</template>

<style>
#app {
  background: url('/flying_landscape.jpg')
    no-repeat center center;
  background-size: cover;
  }
</style>