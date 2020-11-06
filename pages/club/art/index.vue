<template>
  <v-app class="club-page">
    <v-container>
      <v-row no-gutters>
        <v-col class="py-12" cols="12">
          <h1 align="center"> 美術部 </h1>
        </v-col>
      </v-row>
    </v-container>
    <v-container fluid style="width: 85%">
      <v-row no-gutters>
        <v-col class="py-12" cols="12">
          <v-col class="pa-2" cols="12">
          <p class="subtitle" align="left"> こちらは、美術部になります!!! </p>
          <p class="subtitle" align="left"> 
            高専の美術部の特徴としては、「とにかく作りたいものを作品にする。」というのをモットーに活動しています。
          </p>
          <p class="subtitle" align="left"> 
            自分の作りたい作品に専念でき、自由なところが高専美術部の良いところだと思います。
          </p>
          <p class="subtitle" align="left"> 
            コロナ対策として部室内の活動人数を制限する中で各部員が作品を作り上げてくれました。
          </p>
          <p class="subtitle" align="left"> 
            今回掲載する作品の中で皆さんにどれか一つでも気に入ってもらえる作品があればとても嬉しいです!!!
          </p>
        </v-col>
        <v-col cols="12">
          <v-layout align-center>
            <v-icon size="35">mdi-menu-right</v-icon>
            <nuxt-link class="mx-3 title" to="/club/art/origami"> 折り紙 </nuxt-link>
          </v-layout>  
        </v-col>
        <v-col cols="12">
          <v-layout align-center>
            <v-icon size="35">mdi-menu-right</v-icon>
            <a class="mx-3 title" href="https://cdn.nitncfes.net/art/notebook.pdf" target=”_blank”> 部誌 </a>
          </v-layout>  
        </v-col>
        <v-col cols="12">
          <v-layout align-center>
            <v-icon size="35">mdi-menu-right</v-icon>
            <nuxt-link class="mx-3 title" to="/club/art/collection"> 作品集 </nuxt-link>
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