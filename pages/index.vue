<template>
  <v-app>
      <v-container
        fluid
        class="top-content"
      >
        <v-row no-gutters>
          <v-col class="pa-2" cols="12">
            <h1 align="center"> オンライン高専祭！ </h1>
          </v-col>
          <v-col class="pa-2" cols="12">
            <h3 align="center"> 今年はすべての企画が本サイトにて公開されます！ </h3>
          </v-col>
          <v-col class="pa-2" cols="12">
            <h3 align="center"> 開催日： 2020年11月7日</h3>
            <h3 align="center"> 動画配信期間： 〜11月14日</h3>
          </v-col>
        </v-row>
      </v-container>
      <v-container
        fluid
        style="width: 85%"
      >
        <h1 align="center"> 注意 </h1>
        <v-row justify="center">
          <v-col class="mx-12 my-6">
            <InfoSquare
              title="学内入構について"
              icon="mdi-minus-circle"
              rgb="#FF3F43"
              description="高専祭開催中は関係者のみが入構でき、一般の方は入構できません。予めご了承ください。"
            />
          </v-col>
          <v-col class="mx-12 my-6">
            <InfoSquare
              title="サイトについて"
              icon="mdi-lan-disconnect"
              rgb="#7F41C0"
              description="サーバーに高負荷をかける行為はおやめください。"
            />
          </v-col>
          <v-col class="mx-12 my-6">
            <InfoSquare
              title="お問い合わせ"
              icon="mdi-email"
              rgb="#40C07F"
              description="高専祭実行委員会へは下記メールアドレスにお問い合わせください。"
            />
          </v-col>
        </v-row>
      </v-container>
  </v-app>
</template>

<script>
import InfoSquare from '@/components/InfoSquare'

export default {
  components: {
    InfoSquare
  },
  data() {
    return {
      top_image: require('@/assets/light-grey-terrazzo.png'),
    }
  } 
}
</script>

<style lang="scss" scoped>
.top-content {
  background: url('~assets/light-grey-terrazzo.png') fixed repeat round;
}
</style>
