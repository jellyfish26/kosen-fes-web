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
            <v-layout justify-center>
              <v-card
                class="enter-school"
                height="300px"
                width="300px"
                outlined
              >
                <v-layout 
                  justify-center
                  class="my-4"
                >
                  <v-list class="pa-0">
                    <v-list-item>
                      <p class="headline mx-auto"> 学内入構について </p>
                    </v-list-item>
                    <v-list-item>
                      <v-icon class="mx-auto" color="#FF3F43" size="100px"> mdi-minus-circle </v-icon>
                    </v-list-item>
                    <v-list-item>
                      <p class="subtitle my-3 mx-2"> 高専祭開催中は関係者のみが入構でき、一般の方は入構できません。予めご了承ください。 </p>
                    </v-list-item>
                  </v-list>
                </v-layout>
              </v-card>
            </v-layout>
          </v-col>
          <v-col class="mx-12 my-6">
            <v-layout justify-center>
              <v-card
                class="attack-server"
                height="300px"
                width="300px"
                outlined
              >
                <v-layout 
                  justify-center
                  class="my-4"
                >
                  <v-list class="pa-0">
                    <v-list-item>
                      <p class="headline mx-auto"> サイトについて </p>
                    </v-list-item>
                    <v-list-item>
                      <v-icon class="mx-auto" color="#7F41C0" size="100px"> mdi-lan-disconnect </v-icon>
                    </v-list-item>
                    <v-list-item>
                      <p class="subtitle my-5 mx-2"> サーバーに負荷をかける行為はおやめください。 </p>
                    </v-list-item>
                  </v-list>
                </v-layout>
              </v-card>
            </v-layout>
          </v-col>
          <v-col class="mx-12 my-6">
            <v-layout justify-center>
              <v-card
                class="contact"
                height="300px"
                width="300px"
                outlined
              >
                <v-layout 
                  justify-center
                  class="my-4"
                >
                  <v-list class="pa-0">
                    <v-list-item>
                      <p class="headline mx-auto"> お問い合わせ </p>
                    </v-list-item>
                    <v-list-item>
                      <v-icon class="mx-auto" color="#40C07F" size="100px"> mdi-email </v-icon>
                    </v-list-item>
                    <v-list-item>
                      <p class="subtitle my-5 mx-2"> 高専祭委員会へは下記メールアドレスにお問い合わせください。 </p>
                    </v-list-item>
                  </v-list>
                </v-layout>
              </v-card>
            </v-layout>
          </v-col>
        </v-row>
      </v-container>
  </v-app>
</template>

<script>

export default {
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

.enter-school {
  border: 5px solid #FF3F43;
}

.attack-server {
  border: 5px solid #7F41C0;
}

.contact {
  border: 5px solid #40C07F;
}
</style>
