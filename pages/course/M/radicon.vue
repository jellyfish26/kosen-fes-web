<template>
  <v-app class="club-page">
    <v-container>
      <v-row no-gutters>
        <v-col class="py-12" cols="12">
          <h1 align="center"> 機械工学科 </h1>
        </v-col>
        <v-col class="py-12" cols="12">
          <h2 align="center"> ラジコンプレーン </h2>
        </v-col>
      </v-row>
    </v-container>
     <v-container style="width: 85%">
      <HLSVideo
        src="https://cdn.nitncfes.net/M/radicon/video.m3u8"
      />
    </v-container>
  </v-app>
</template>

<style scoped>
.club-page {
  background: url('~assets/ep_naturalwhite.png') fixed repeat round;
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