<template>
  <v-app class="club-page">
    <v-container>
      <v-row no-gutters>
        <v-col class="py-12" cols="12">
          <h1 align="center"> 陸上競技部 </h1>
        </v-col>
      </v-row>
    </v-container>
    <v-container style="width: 85%">
      <HLSVideo
        src="https://cdn.nitncfes.net/ground/main/video.m3u8"
      />
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