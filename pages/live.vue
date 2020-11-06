<template>
  <v-app class="live-page">
    <v-container>
      <v-row no-gutters>
        <v-col class="py-12" cols="12">
          <h1 align="center" class="white--text"> 企画(ライブ配信) </h1>
        </v-col>
      </v-row>
    </v-container>
    <v-container style="width: 85%">
       <v-layout justify-center>
         <YoutubeVideo
          id="lXuiNmpXu7E"
        />
       </v-layout>
    </v-container>
  </v-app>
</template>

<style scoped>
.live-page {
  background: url('~assets/footer_lodyas.png') fixed repeat round;
}
</style>