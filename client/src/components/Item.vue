<template>
    <v-card  class="mb-2" color="primary" dark hover max-height="600">
      <v-card-title class="left">
        <v-icon left>mdi-gender-male</v-icon>
        <span class="Regular font-weight-light">Đại học Khoa Học Tự Nhiên</span>
      </v-card-title>

      <v-card-text
        class="body-2 font-weight-bold d-flex text-md-left text-sm-left"
      >"Turns out semicolon-less style is easier and safer in TS because mo.Turns out semicolon-less style is easier and safer in TS because mo."</v-card-text>

      <v-card-actions>
        <v-list-tile class="grow">
          <v-list-tile-avatar color="grey darken-3">
            <v-img
              class="elevation-6"
              src="https://avataaars.io/"
            ></v-img>
          </v-list-tile-avatar>

          <v-list-tile-content>
            <v-list-tile-title :class="this.$vuetify.breakpoint.mdAndUp?'font-weight-medium text-name':'font-weight-medium'">Evan You</v-list-tile-title>
             <v-list-tile-title class="caption font-weight-light">HCM</v-list-tile-title>
          </v-list-tile-content>

          <v-layout align-center justify-end>
            <v-btn icon><v-icon class="mr-1">mdi-heart</v-icon></v-btn>
            <span class="subheading mr-1">256</span>
            <span class="mr-2"></span>
              <v-btn icon> <v-icon class="mr-1">mdi-information</v-icon></v-btn>
          </v-layout>
        </v-list-tile>
      </v-card-actions>
    </v-card>
</template>

<script>
export default {
  data: () => ({})
};
</script>

<style scoped>
.text-name{
    overflow: hidden;
    width:77px;
}
</style>
