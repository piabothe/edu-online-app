<template>
  <div>
    <v-container>
      <v-layout align-center>
        <v-flex>
          <h3 class="display-3">Overview-Header</h3>
          <span class="subheading">Overview-Intro</span>
          <v-divider class="my-3"></v-divider>
          <div class="title mb-3">Overview-Content</div>
          <v-timeline>
            <v-timeline-item v-for="n in 4" :key="n" color="#0065BD" large>
              <v-card class="elevation-2">
                <v-card-title class="headline">Kurs-/Kapiteltitel</v-card-title>
                <v-card-text>Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae.</v-card-text>
              </v-card>
            </v-timeline-item>
          </v-timeline>
        </v-flex>
      </v-layout>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "overview",
  props: {
    msg: String
  }
};
</script>

<style>
</style>