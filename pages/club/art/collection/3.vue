<template>
  <v-app class="club-page">
    <v-container>
      <v-row no-gutters>
        <v-col class="py-12" cols="12">
          <h1 align="center"> 美術部 </h1>
        </v-col>
        <v-col class="py-12" cols="12">
          <h2 align="center"> ケッテンクラート </h2>
        </v-col>
      </v-row>
    </v-container>
    <v-container fluid style="width: 85%">
      <v-row no-gutters>
        <v-col class="py-3" cols="12" >
          <v-layout justify-center>
            <v-img
              src="https://cdn.nitncfes.net/art/collection/3/first.jpg"
            > </v-img>
          </v-layout>
        </v-col>
        <v-col class="py-3" cols="12" >
          <v-layout justify-center>
            <v-img
              src="https://cdn.nitncfes.net/art/collection/3/second.jpg"
            > </v-img>
          </v-layout>
        </v-col>
        <v-col cols="12">
           <p class="py-3 title font-weight-bold" align="center"> 作品の説明 </p>
        </v-col>
        <v-col class="py-3" cols="12">
          <p class="subtitle" align="left"> 
            ほぼ紙でケッテンクラートを作成しました。塗装しているのでわかりにくいと思いますが 
            1つの板を作成するのに少なくとも4枚の同じ型の工作用紙を重ねています。車輪に関しては、
            1つの車輪を作成するのに16枚使用しているので全部の車輪を作成するのに100枚近くの同じ型をサークルカッターで切り出しています。
            ばねの部分は、つまようじにはんだを巻き付けて似せています。とにかく製作するのが大変でした。(笑) 
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