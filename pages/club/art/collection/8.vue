<template>
  <v-app class="club-page">
    <v-container>
      <v-row no-gutters>
        <v-col class="py-12" cols="12">
          <h1 align="center"> 美術部 </h1>
        </v-col>
        <v-col class="py-12" cols="12">
          <h2 align="center"> イラスト </h2>
        </v-col>
      </v-row>
    </v-container>
    <v-container fluid style="width: 85%">
      <v-row no-gutters>
        <v-col class="py-3" cols="12" >
          <v-layout justify-center>
            <v-img
              src="https://cdn.nitncfes.net/art/collection/8/first.jpg"
            > </v-img>
          </v-layout>
        </v-col>
        <v-col cols="12">
           <p class="py-3 title font-weight-bold" align="center"> 作品の説明 </p>
        </v-col>
        <v-col class="py-3" cols="12">
          <p class="subtitle" align="left"> 
            設定：遊びに降りてきた天使が人に毒されて堕天してしまった  
          </p>
          <p class="subtitle" align="left"> 
            中性的な顔、ダークな雰囲気など好みを詰め込みました。 
          </p>
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
import HLSVideo from '@/components/HLSVideo'

export default {
  components: {
    HLSVideo
  },
  data() {
    return {
    }
  }
}
</script>