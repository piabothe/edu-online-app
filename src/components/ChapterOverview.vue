<template>
  <div>
    <v-container>
      <v-layout align-center>
        <v-flex>
          <h3 class="display-3">ChapterOverview-Header</h3>
          <span class="subheading">ChapterOverview-Intro</span>
          <v-divider class="my-3"></v-divider>
          <v-timeline>
            <v-timeline-item v-for="n in 4" :key="n" color="#0065BD" large>
              <v-card class="elevation-2">
                <v-card-title class="headline">Kapiteltitel</v-card-title>
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
  name: "chapterOverview",
  props: {
    msg: String
  }
};
</script>

<style>
</style>