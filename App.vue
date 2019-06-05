<template>
  <div id="app">
    <v-app id="inspire">
      <v-responsive>
        <v-layout xs12>
          <v-toolbar>
            <v-toolbar-title>Title</v-toolbar-title>
            <v-spacer></v-spacer>
            <v-toolbar-items class="hidden-sm-and-down">
              <v-btn flat>Link One</v-btn>
              <v-btn flat>Link Two</v-btn>
              <v-btn flat>Link Three</v-btn>
            </v-toolbar-items>
          </v-toolbar>
        </v-layout>

        <v-container>
          <v-layout align-center xs12>
            <v-flex>
              <h3 class="display-3">{{title}}</h3>
              <span
                class="subheading"
              >Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae.Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae.</span>
              <v-divider class="my-3"></v-divider>
              <div class="title mb-3">Neu hier? Registriere dich ganz ohne E-Mail-Adresse!</div><Login v-show=/>
              <Home v-show/>
              <Overview v-show/>
              <Overview v-show/>
              <Chapter v-show/>
            </v-flex>
          </v-layout>
        </v-container>

        <v-footer class="pa-3" color="#0065BD" style="color:white">
          <v-spacer></v-spacer>
          <div>&copy; {{ new Date().getFullYear() }}</div>
        </v-footer>
      </v-responsive>
    </v-app>
  </div>
</template>

<script>
import Login from "./components/Login";
import Home from "./components/Home";
import Overview from "./components/Overview";
import Chapter from "./components/Chapter";

export default {
  name: "App",
  components: {
    Login: Login,
    Home: Home,
    Overview: Overview,
    Chapter: Chapter
  },
  data() {
    return {
      title: "Hi!"
    };
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
