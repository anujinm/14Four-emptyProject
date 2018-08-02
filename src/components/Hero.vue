<template lang="pug">
  .hero
    //- TODO: demonstrate v-on v-bind v-for v-if {{ }}, scoped styles, transitions
    h2 Hero
</template>

<script>
import { mapActions, mapState } from 'vuex'
import debug from 'debug'
let log = debug('component:Hero')
export default {
  name: 'hero',
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
    ...mapState('tasks', {
      tasksSorted: state => state.all.slice().sort((a, b) => a.title.localeCompare(b.title))
    })
  },
  methods: {
    ...mapActions('tasks', [
      'syncTask',
      'setActiveTask'
    ]) // ,
    // toggleComplete (task) {
    //   task.isComplete = !task.isComplete
    // }
  },
  components: {
  }
}
</script>

<style scoped lang="scss">
@import "../styles/_variables";
@import "../styles/_mixins";
.hero {
}
</style>
