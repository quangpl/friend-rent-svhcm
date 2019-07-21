<template>
  <v-app id="inspire">
    <v-navigation-drawer v-model="drawer" app temporary width="180">
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
      <v-btn @click="drawer=!drawer" icon>
        <v-icon>menu</v-icon>
      </v-btn>
      <v-toolbar-title>
        <v-icon class="mr-2">search</v-icon>MyFriend
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <div v-if="this.$vuetify.breakpoint.mdAndUp">
        <v-btn icon class="mr-5 mb-4 mt-2">
          <v-btn color="error">Đăng cho thuê</v-btn>
        </v-btn>
      </div>
      <div v-if="this.$vuetify.breakpoint.smAndDown">
         <v-btn fab dark small color="white">
      <v-icon dark color="indigo">add</v-icon>
    </v-btn>
      </div>
      <v-badge color="red" overlap>
        <template v-slot:badge>
          <span>1</span>
        </template>
       <v-avatar size="36px" :class="this.$vuetify.breakpoint.mdAndUp?'ml-4':'ml-2'">
        <img src="https://avatars0.githubusercontent.com/u/9064066?v=4&s=460" alt="Avatar" />
      </v-avatar>
      </v-badge>
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
