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
      <v-container fluid>
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
        <v-layout class="my-10" style="height: 100%" justify-center align-end>
          <v-btn
            class="mx-2"
            fab
            dark
            color="#1DA1F2"
            href="https://twitter.com/nara_kousensai"
            target="_blank"
          >
            <v-icon>
              mdi-twitter
            </v-icon>
          </v-btn>
        </v-layout>
      </v-container>
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
        },
        {
          icon: 'mdi-magnify',
          title: '実行委員会より',
          to: '/about'
        },
        {
          icon: 'mdi-biathlon',
          title: '部活科展',
          to: '/club'
        },
        {
          icon: 'mdi-school',
          title: '学科展',
          to: '/course'
        },
        {
          icon: 'mdi-animation-play',
          title: '企画(ライブ配信)',
          to: '/live'
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