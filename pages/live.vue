<template>
  <v-app class="live-page">
    <v-container>
      <v-row no-gutters>
        <v-col class="pa-2" cols="12">
          <p class="display-2 white--text" align="center"> Coming Soon... </p>
        </v-col>
        <v-col class="pa-2" cols="12">
          <h1 class="white--text" align="center"> 公開までしばらくお待ちください。 </h1>
        </v-col>
        <v-col class="pa-2" cols="12">
          <div align="center">
            <nuxt-link class="subtitle white--text" to="/"> トップページへ戻る。 </nuxt-link>
          </div>
        </v-col>
      </v-row>
      
    </v-container>
  </v-app>
</template>

<style scoped>
.live-page {
  background: url('~assets/footer_lodyas.png') fixed repeat round;
}
</style>