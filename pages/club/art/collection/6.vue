<template>
  <v-app class="club-page">
    <v-container>
      <v-row no-gutters>
        <v-col class="py-12" cols="12">
          <h1 align="center"> 美術部 </h1>
        </v-col>
        <v-col class="py-12" cols="12">
          <h2 align="center"> 恐竜 </h2>
        </v-col>
      </v-row>
    </v-container>
    <v-container fluid style="width: 85%">
      <v-row no-gutters>
        <v-col class="py-3" cols="12" >
          <v-layout justify-center>
            <v-img
              src="https://cdn.nitncfes.net/art/collection/6/first.jpg"
            > </v-img>
          </v-layout>
        </v-col>
        <v-col cols="12">
           <p class="py-3 title font-weight-bold" align="center"> 作品の説明 </p>
        </v-col>
        <v-col class="py-3" cols="12">
          <p class="subtitle" align="left"> 
            折り紙のギガノトサウルスです。 
            Shuki Katoさん創作で、折り図を見ながら作りました。 
            400近い工程で、24本の歯やがっしりとした脚などを折りあげていきます。 
            今回は54cm四方の洋紙で折りました。 
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