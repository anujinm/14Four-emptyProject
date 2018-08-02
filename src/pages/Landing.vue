<template lang="pug">
  .landing
    h1 Landing Page
</template>

<script>
import debug from 'debug'
let log = debug('component:Landing')
export default {
  name: 'landing',
  props: [],
  data () {
    return {
    }
  },
  beforeCreate: function () {
  },
  mounted: function () {
    log('Mounted')
  },
  computed: {
  },
  methods: {
  },
  components: {
  }
}
</script>

<style scoped lang="scss">
@import "../styles/_variables";
@import "../styles/_mixins";
.landing {
  
}
</style>
