<template>
<div>
    <v-container grid-list-md text-xs-center class="mt-5">
    <v-layout row wrap>
      <v-flex xs12 sm6 md4 lg3>
        <Item/>
      </v-flex>
      <v-flex xs12 sm6 md4 lg3>
        <Item/>
      </v-flex>
      <v-flex xs12 sm6 md4 lg3>
        <Item/>
      </v-flex>
      <v-flex xs12 sm6 md4 lg3>
        <Item/>
      </v-flex>
      <v-flex xs12 sm6 md4 lg3>
        <Item/>
      </v-flex>
      <v-flex xs12 sm6 md4 lg3>
        <Item/>
      </v-flex>
      
    </v-layout>
  </v-container>
</div>

</template>
<script>
import Item from "./Item";
export default {
  components: {
    Item
  },
  data: () => ({
    card_text:
      "Lorem ipsum dolor sit amet, brute iriure accusata ne mea. Eos suavitate referrentur ad, te duo agam libris qualisque, utroque quaestio accommodare no qui. Et percipit laboramus usu, no invidunt verterem nominati mel. Dolorem ancillae an mei, ut putant invenire splendide mel, ea nec propriae adipisci. Ignota salutandi accusamus in sed, et per malis fuisset, qui id ludus appareat."
  })
};
</script>

<style>
</style>
