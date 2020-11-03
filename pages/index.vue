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
          <h3 align="center"> 今年はすべての展示が本サイトにて公開されます！ </h3>
        </v-col>
        <v-col class="pa-2" cols="12">
          <h3 align="center"> 開催日： 2020年11月7日</h3>
          <h3 align="center"> 展示配信期間： 〜11月14日</h3>
        </v-col>
      </v-row>
    </v-container>
    <v-layout class="theme">
      <v-container fluid style="width: 85%">
        <v-row no-gutters>
          <v-col class="pa-2" cols="12">
            <h1 align="center"> テーマ </h1>
          </v-col>
          <v-col class="pa-2" cols="12">
            <h2 align="center" class="font-weight-black"> 「高専CUBE　～色とりどりに染め上げよう～」 </h2>
          </v-col>
        </v-row>
        <v-row no-gutters justify="center" align="center">
          <v-col class="pa-2">
            <v-layout justify-center>
              <v-img
                max-width="320px"
                :src="theme_image"
              > </v-img>
            </v-layout>
          </v-col>
          <v-col class="py-2 px-2">
            <p class="title" align="left"> 今年のテーマは「高専CUBE　～色とりどりに染め上げよう～」に決定しました！ </p>
            <p class="title" align="left"> それぞれの個性（色）でいくつもの面を染め上げて，ひとつの大きなキューブを作り上げようという思いが込められています． </p>
            <p class="title" align="left"> それぞれの個性を生かした展示をお楽しみください！ </p>
          </v-col>
        </v-row>
      </v-container>
    </v-layout>
    <v-container
      fluid
      style="width: 85%"
    >
      <h1 align="center"> 注意 </h1>
      <v-row justify="center">
        <v-col class="mx-12 my-6">
          <WarnSquare
            title="学内入構について"
            icon="mdi-minus-circle"
            rgb="#FF3F43"
            description="高専祭開催中は関係者のみ入構が許可されており、一般の方は入構できません。予めご了承ください。"
          />
        </v-col>
        <v-col class="mx-12 my-6">
          <WarnSquare
            title="サイトについて"
            icon="mdi-lan-disconnect"
            rgb="#7F41C0"
            description="サーバーに高負荷をかける行為はおやめください。"
          />
        </v-col>
        <v-col class="mx-12 my-6">
          <WarnSquare
            title="お問い合わせ"
            icon="mdi-email"
            rgb="#40C07F"
            description="高専祭実行委員会へは下記にお問い合わせください。"
            url="https://www.nara-k.ac.jp/inquiry/"
            urlDesc="奈良高専 学生課学生係"
          />
        </v-col>
      </v-row>
    </v-container>
    <v-layout class="fes-fun">
      <v-container fluid style="width: 85%">
        <h1 class="white--text" align="center"> オンラインを楽しむ！ </h1>
        <v-row justify="center">
          <v-col class="mx-12 my-3">
            <InfoSquare
              title="実行委員会より"
              icon="mdi-magnify"
              link="about"
            />
          </v-col>
          <v-col class="mx-12 my-3">
            <InfoSquare
              title="部活科展"
              icon="mdi-biathlon"
              link="club"
            />
          </v-col>
        </v-row>
        <v-row justify="center">
          <v-col class="mx-12 my-3">
            <InfoSquare
              title="学科展"
              icon="mdi-school"
              link="course"
            />
          </v-col>
          <v-col class="mx-12 my-3">
            <InfoSquare
              title="企画(ライブ配信)"
              icon="mdi-animation-play"
              link="live"
            />
          </v-col>
        </v-row>
      </v-container>
    </v-layout>
  </v-app>
</template>

<script>
import WarnSquare from '@/components/WarnSquare'
import InfoSquare from '@/components/InfoSquare'

export default {
  components: {
    WarnSquare,
    InfoSquare
  },
  data() {
    return {
      top_image: require('@/assets/light-grey-terrazzo.png'),
      theme_image: require('@/assets/theme_illust.png'),
    }
  } 
}
</script>

<style lang="scss" scoped>
.top-content {
  background: url('~assets/light-grey-terrazzo.png') fixed repeat round;
}

.fes-fun {
  background: url('~assets/low_contrast_linen.png') fixed repeat round;
}

.theme {
  background-color: #F5DEB3;
}
</style>
