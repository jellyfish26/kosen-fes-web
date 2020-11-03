<template>
<vue-core-video-player :core="HLSCore" :src="src" />
</template>


<script>
import HLSCore from '@core-player/playcore-hls'

export default {
  props: {
    src: {
      type: String,
      default: ''
    },
  },
  data() {
    return {
      HLSCore
    }
  }
}
</script>