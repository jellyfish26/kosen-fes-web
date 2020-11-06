<template>
  <v-app class="course-page">
    <v-container>
      <v-row no-gutters>
        <v-col class="py-12" cols="12">
          <h1 align="center"> 学科展 </h1>
        </v-col>
      </v-row>
    </v-container>
    <v-container style="width: 85%">
      <v-row>
        <v-col class="my-6" v-for="item in course" :key="item.name">
          <CoursePanel
            :title="item.name"
            :description="item.description"
            :url="item.url"
            :href="item.href"
            :rgb="item.rgb"
          />
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

<script>
import CoursePanel from '@/components/CoursePanel'

export default {
  components: {
    CoursePanel
  },
  data() {
    return {
      course: [
        {
          name: "機械工学科",
          description: "学科+課外活動の紹介　〜オモイをカタチに〜",
          rgb: "#ff7a7a",
          url: "/course/M/"
        },
        {
          name: "電気工学科",
          description: "電気科展では、これまでに展示してきた展示品に加え、新しく展示する企画もあり、いろとりどりの展示品が並ぶ科展となっております。特設HPと併せて、是非ご覧ください！！！",
          rgb: "#ffe77a",
          href: "https://sites.google.com/view/colorful-erectric-exhibits"
        },
        {
          name: "電子制御工学科",
          description: "課題解決型実験の動画と電子工作",
          rgb: "#7fff7a",
          url: "/course/S/"
        },
        {
          name: "情報工学科",
          description: "みんなで遊ぶ放置ゲーム（鹿煎餅増やしゲーム）AIと対戦，カスタム可能オセロ",
          rgb: "#7ac1ff",
          url: "/course/I/"
        },
        {
          name: "物質科学工学科",
          description: "いろいろな実験を見てみよう！楽しい実験がいっぱい(^^♪ 分かりやすい解説付きです．",
          rgb: "#9e7aff",
          url: "/course/C/"
        }
      ]
    }
  }
}
</script>