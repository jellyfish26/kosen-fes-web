<template>
  <v-app class="club-page">
    <v-container>
      <v-row no-gutters>
        <v-col class="py-12" cols="12">
          <h1 align="center"> クイズ研究会 </h1>
        </v-col>
      </v-row>
    </v-container>
    <v-container style="width: 85%">
      <v-row no-gutters>
        <v-col cols="12">
          <v-layout align-center>
            <v-icon size="35">mdi-menu-right</v-icon>
            <a class="mx-3 title" href="https://cdn.nitncfes.net/quiz/quiz.pdf" target=”_blank”> クイズ！ </a>
          </v-layout>  
        </v-col>
        <v-col cols="12">
          <v-layout align-center>
            <v-icon size="35">mdi-menu-right</v-icon>
            <a class="mx-3 title" href="https://cdn.nitncfes.net/quiz/answer.pdf" target=”_blank”> 答え </a>
          </v-layout>  
        </v-col>
      </v-row>
    </v-container>
  </v-app>
</template>

<style scoped>
.club-page {
  background: url('~assets/struckaxiom.png') fixed repeat round;
}
</style>

<script>
import pdf from 'vue-pdf'

export default {
  components: {
    pdf
  },
  data() {
    return {
    }
  },
}
</script>