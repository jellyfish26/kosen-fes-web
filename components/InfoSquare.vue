<template>
  <v-layout justify-center>
    <v-card
      :style="{ 'border': '5px solid #40C0FF'}"
      height="100px"
      width="100%"
      min-width="250px"
      hover
      nuxt
      :to="link"
    >
      <v-layout
        class="ml-3 my-3"
      >
        <v-icon class="mx-auto" color="#40C0FF" size="40px"> {{ icon }}</v-icon>
        <v-divider
          class="my-3 mx-5"
          vertical
        ></v-divider>
        <v-spacer />
        <h3 class="my-5"> {{ title }} </h3>
        <v-spacer />
      </v-layout>
    </v-card>
  </v-layout>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: 'hogehoge'
    },
    icon: {
      type: String,
      default: 'mdi-minus-circle'
    },
    rgb: {
      type: String,
      default: '#000000'
    },
    description: {
      type: String, 
      default: 'fugafuga'
    },
    link: {
      type: String,
      default: '/'
    }
  }
}
</script>