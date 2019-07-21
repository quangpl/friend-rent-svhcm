<template>
  <v-app id="inspire">
    <v-navigation-drawer
      v-model="drawer"
      app
      temporary
      
    >
      <v-list dense>
        <v-list-tile>
          <v-list-tile-action>
            <v-icon>home</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title>Home</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
        <v-list-tile>
          <v-list-tile-action>
            <v-icon>contact_mail</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title>Contact</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>
    <v-toolbar color="indigo" dark fixed app>
      <v-btn @click="drawer=!drawer" icon><v-icon>menu</v-icon></v-btn>
      <v-toolbar-title><v-icon>search</v-icon>MyFriend</v-toolbar-title>
    </v-toolbar>
  </v-app>
</template>
<script>
export default {
  data: () => ({
    drawer: null,
    items: [
      { title: "Home", icon: "dashboard" },
      { title: "About", icon: "question_answer" }
    ]
  })
};
</script>

<style>
</style>
