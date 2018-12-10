<template>
  <div>
    {{ msg }}
  </div>
</template>

<script>
// import store from '@/store'
import { mapState } from 'vuex'

export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  computed: {
    ...mapState({
      msg: state => state.msg
    })
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
