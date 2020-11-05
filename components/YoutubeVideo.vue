<template>
<v-card height="600px" width="100%">
  <iframe
    height="100%"
    width="100%"
    :src="'https://www.youtube.com/embed/' + id"
    frameborder="0"
    allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen
  ></iframe>
</v-card>
</template>


<script>

export default {
  props: {
    id: {
      type: Array
    },
  }
}
</script>