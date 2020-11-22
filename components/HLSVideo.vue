<template>
<vue-core-video-player :core="HLSCore" :src="src" autoplay/>
</template>


<script>
import HLSCore from '@core-player/playcore-hls'

export default {
  props: {
    src: {
      type: Array
    },
  },
  data() {
    return {
      HLSCore
    }
  },
}
</script>