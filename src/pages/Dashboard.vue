<template lang="pug">
  .dashboard
    h1 Dashboard Page
    hero
</template>

<script>
import hero from '@/components/Hero'
import debug from 'debug'
let log = debug('component:Dashboard')
export default {
  name: 'dashboard',
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
    'hero': hero
  }
}
</script>

<style scoped lang="scss">
@import "../styles/_variables";
@import "../styles/_mixins";
.dashboard {
  
}
</style>
