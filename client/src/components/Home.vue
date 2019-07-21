<template>
<v-app>
<v-container>
<v-layout>
  <HomeBar />
  <HomeContent />
</v-layout>
</v-container>
</v-app>


</template>

<script>
import HomeBar from "./HomeBar";
import HomeContent from "./HomeContent";

export default {
  components: {
    HomeBar,
    HomeContent
  },
  data: () => ({})
};
</script>

<style>
</style>
