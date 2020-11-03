<template>
  <v-app dark>
    <v-navigation-drawer
      v-if="this.$vuetify.breakpoint.width < 1264"
      v-model="drawer"
      right
      fixed
      width="300"
      :src="navigation_image"
      app
    >
      <NavigateDrawer />
    </v-navigation-drawer>
    <v-navigation-drawer
      v-else
      v-model="drawer"
      fixed
      width="300"
      :src="navigation_image"
      app
    >
      <NavigateDrawer />
    </v-navigation-drawer>
    <v-app-bar
      v-if="this.$vuetify.breakpoint.width < 1264"
      clipped-right
      fixed
      :src="navigation_image"
      app
    >
      <h3> 第54回奈良高専祭 </h3>
      <v-spacer/>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
    </v-app-bar>
    <v-main>
      <nuxt />
    </v-main>
    <v-footer>
      <span>&copy; 2020 情報処理研究会</span>
    </v-footer>
  </v-app>
</template>

<script>
import Vuetify from 'vuetify'
import NavigateDrawer from '@/components/NavigateDrawer'

export default {
  components: {
    NavigateDrawer
  },
  data () {
    return {
      clipped: false,
      fixed: false,
      drawer: false,
      navigation_image: require('@/assets/retina_wood.png'),
      right: true,
      title: 'Vuetify.js'
    }
  },
  mounted() {
    this.drawer = this.$vuetify.breakpoint.width >= 1264
  }
  
}
</script>