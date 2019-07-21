<template>
<v-layout class="mt-5 white">
    <v-combobox
      v-model="select"
      :items="items"
      label="Bạn đang tìm..."
    ></v-combobox>
</v-layout>
</template>

<script>
export default {
  data: () => ({
    select: "Nam",
    items: ["Nam","Nữ","Khác","Gì cũng được"]
  })
};
</script>

<style>
</style>
