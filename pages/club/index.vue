<template>
  <v-app class="club-page">
    <v-container>
      <v-row no-gutters>
        <v-col class="py-12" cols="12">
          <h1 align="center"> 部活科展 </h1>
        </v-col>
      </v-row>
    </v-container>
    <v-container style="width: 85%">
      <v-row>
        <v-col cols="12">
          <v-layout>
            <v-icon size="35">mdi-run-fast</v-icon>
            <h2 class="mx-3"> 運動部 </h2>
          </v-layout>
        </v-col>
        <v-col class="mx-3" v-for="item in active_clubs" :key="item.name">
          <Panel
            :title="item.name"
            :description="item.description"
            :url="item.url"
          />
        </v-col>
      </v-row>
    </v-container>
    <v-container style="width: 85%">
      <v-row>
        <v-col cols="12">
          <v-layout>
            <v-icon size="35" color="#6FEA7C">mdi-lightbulb-on</v-icon>
            <h2 class="mx-3"> 文化部 </h2>
          </v-layout>
        </v-col>
        <v-col class="mx-3" v-for="item in culture_clubs" :key="item.name">
          <Panel
            :title="item.name"
            :description="item.description"
            :url="item.url"
            rgb="#6FEA7C"
          />
        </v-col>
      </v-row>
    </v-container>
    <v-container style="width: 85%">
      <v-row>
        <v-col cols="12">
          <v-layout>
            <v-icon size="35" color="#7AC1FF ">mdi-emoticon-outline</v-icon>
            <h2 class="mx-3"> 同好会 / 有志 </h2>
          </v-layout>
        </v-col>
        <v-col class="mx-3" v-for="item in other" :key="item.name">
          <Panel
            :title="item.name"
            :description="item.description"
            :url="item.url"
            :href="item.href"
            rgb="#7AC1FF "
          />
        </v-col>
      </v-row>
    </v-container>
  </v-app>
</template>

<style scoped>
.club-page {
  background: url('~assets/struckaxiom.png') fixed repeat round;
}
</style>

<script>
import Panel from '@/components/Panel'

export default {
  components: {
    Panel
  },
  data() {
    return {
      active_clubs: [
        {
          name: "陸上競技部",
          description: "陸上競技の種目紹介と普段の練習風景を動画にしました！3分くらいの短い動画なので見て頂けると嬉しいです！",
          url: "/club/ground"
        },
        {
          name: "合気道部",
          description: "多彩な技で、迫力のある技紹介動画と合気道部について一目でわかるポスターを作成しました。ぜひご覧ください！",
          url: "/club/aikido"
        },
        {
          name: "少林寺拳法部",
          description: "少林寺拳法の紹介ビデオです。",
          url: "/club/shorinji_kempo"
        },
        {
          name: "ソフトテニス部",
          description: "部活紹介！！！",
          url: "/club/soft_tennis"
        },
        {
          name: "弓道部",
          description: "KENTO福田の弓道実況",
          url: "/club/japanese_archery"
        },
        {
          name: "硬式テニス部",
          description: "〜Come On！〜活動紹介ポスターへようこそ",
          url: "/club/hard_tennis"
        },
        {
          name: "水泳部",
          description: "水泳部のPR動画（水泳部の一年間，部員インタビュー，バカッコイイ水泳部）",
          url: "/club/swimming"
        },
      ],
      culture_clubs: [
        {
          name: "美術部",
          description: "各部員が自分の「得意」や、「好きなこと」で、イラスト･絵画・工作を作成しました。",
          url: "/club/art"
        },
        {
          name: "情報処理研究会",
          description: "本サイトを作成しました！",
          url: "/"
        },
        {
          name: "機械研究会",
          description: "個人が製作したルアーや絵、模型等を文字付きで公開",
          url: "/club/mechanical"
        },
      ],
      other: [
        {
          name: "手芸同好会",
          description: "作品の写真と活動の動画",
          url: "/club/handicraft"
        },
        {
          name: "クイズ研究会",
          description: "簡単な四択クイズです",
          url: "/club/quiz"
        },
        {
          name: "数学同好会",
          description: "数学同好会は，マンデルブロ集合の紹介，ギャラリー，そして実際にマンデルブロ集合の世界に入り込めるシュミレーターを提供します．",
          href: "https://mandelbrot.nitncfes.net/"
        },
        {
          name: "合唱同好会",
          description: "合唱同好会紹介",
          url: "/club/chorus"
        },
        {
          name: "生協学生同好会",
          description: "生協同好会について，同好会紹介",
          url: "/club/coop"
        },
        {
          name: "3年情報工学科",
          description: "映像とVRで体感する仮想コンテンツ",
          href: "https://3info.nitncfes.net"
        },
        {
          name: "1年情報工学科",
          description: "新種のパズルゲーム「Lian」",
          url: "/club/1_info"
        },
        {
          name: "図書委員会",
          description: "新図書館とおすすめの本",
          url: "/club/library"
        },
        {
          name: "高専祭実行委員会",
          description: "学内施設(ファブスペース)の紹介",
          url: "/club/kosensai"
        },
      ]
    }
  }
}
</script>
