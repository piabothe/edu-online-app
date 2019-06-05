<template>
  <v-layout align-center>
    <v-flex xs6>
      <v-card>
        <div style="padding:20px">
          <v-text-field label="Benutzername"></v-text-field>
          <v-text-field label="Passwort" type="password"></v-text-field>

          <v-btn color="#0065BD" large style="color: white">Login</v-btn>
          <v-btn color="#A2AD00" large>Registrieren</v-btn>
        </div>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>
export default {
  name: "login",
  props: {
    msg: String
  }
};
</script>

<style>
</style>