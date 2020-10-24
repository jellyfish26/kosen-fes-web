<template>
  <v-app dark>
    <v-navigation-drawer
      v-model="drawer"
      right
      fixed
      width="300"
      :src="navigation_image"
      app
    >
      <v-list>
        <v-list-item>
          <v-list-item-content>
            <v-list-item-title class="title">
              第54回
              <h3> 奈良高専祭 </h3>
            </v-list-item-title>
            <v-list-item-subtitle>
              「LINK ~繋がる，広がる，最先端！~」
            </v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
        >
          
          <v-list-item-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
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

export default {
  data () {
    return {
      clipped: false,
      fixed: false,
      drawer: false,
      navigation_image: require('@/assets/retina_wood.png'),
      items: [
        {
          icon: 'mdi-home',
          title: 'トップページ',
          to: '/'
        }
      ],
      right: true,
      title: 'Vuetify.js'
    }
  },
  mounted() {
    this.drawer = this.$vuetify.breakpoint.width >= 1264
  }
  
}
</script>
