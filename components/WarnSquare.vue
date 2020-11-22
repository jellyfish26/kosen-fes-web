<template>
  <v-layout justify-center>
    <v-card
      :style="{ 'border': '5px solid ' + rgb}"
      height="100%"
      min-height="310px"
      width="310px"
      outlined
    >
      <v-layout 
        justify-center
        class="my-4"
      >
        <v-list class="pa-0">
          <v-list-item>
            <p class="headline mx-auto"> {{ title }} </p>
          </v-list-item>
          <v-list-item>
            <v-icon class="mx-auto" :color="rgb" size="100px"> {{ icon }}</v-icon>
          </v-list-item>
          <v-list-item>
            <p class="subtitle my-3 mx-2"> {{ description }} </p>
          </v-list-item>
          <v-list-item v-if="url != ''">
            <a class="mx-2" :href="url" target=”_blank”> {{ urlDesc }} </a>
          </v-list-item>
        </v-list>
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
      default: "fugafuga"
    },
    url: {
      type: String, 
      default: ""
    },
    urlDesc: {
      type: String, 
      default: ""
    }
  }
}
</script>