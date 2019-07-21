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
import TheFilter from "./TheFilter";

export default {
  components: {
    HomeBar,
    HomeContent,
    TheFilter
  },
  data: () => ({}),
};
</script>

<style>
</style>
