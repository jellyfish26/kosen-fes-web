<template>
  <v-container fluid>
    <v-list>
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title class="title">
            第54回
            <h3> 奈良高専祭 </h3>
          </v-list-item-title>
          <v-list-item-subtitle>
            LINK ~繋がる，広がる，最先端！~
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
</template>

<script>
export default {
  data() {
    return {
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
    }
  }
}
</script>