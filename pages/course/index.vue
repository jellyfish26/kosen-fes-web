<template>
  <v-app class="course-page">
    <v-container>
      <v-row no-gutters>
        <v-col class="pa-2" cols="12">
          <p class="display-2" align="center"> Coming Soon... </p>
        </v-col>
        <v-col class="pa-2" cols="12">
          <h1 align="center"> 公開までしばらくお待ちください。 </h1>
        </v-col>
        <v-col class="pa-2" cols="12">
          <div align="center">
            <nuxt-link class="subtitle" to="/"> トップページへ戻る。 </nuxt-link>
          </div>
        </v-col>
      </v-row>
      
    </v-container>
  </v-app>
</template>

<style scoped>
.course-page {
  background: url('~assets/ep_naturalwhite.png') fixed repeat round;
}
</style>