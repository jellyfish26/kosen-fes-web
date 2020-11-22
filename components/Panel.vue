<template>
  <v-layout justify-center>
    <v-card
      :style="{ 'border': '5px solid ' + rgb}"
      height="100%"
      min-height="250px"
      width="300px"
      nuxt
      hover
      :to="url"
      :href="href"
    >
      <v-layout 
        justify-center
        class="my-4"
      >
        <p class="my-6 headline font-weight-bold"> {{ title }}</p>
      </v-layout>
      <hr class="mx-6 divisor" />
      <p class="mx-4 my-4"> {{ description}} </p>
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
      default: '#778899'
    },
    description: {
      type: String, 
      default: "fugafuga"
    },
    url: {
      type: String, 
      default: ""
    },
    href: {
      type: String, 
      default: ""
    }
  }
}
</script>

<style lang="scss" scoped>
.divisor{
	border-top: 3px solid #8c8b8b;
}
</style>