<template>
  <div id="app">
    <Loader :isshow="getShowLoading" loaderbackground="rgba(0,0,0,0.3)"></Loader>
  </div>
</template>

<script>
import Loader from './components/common/loader/loader'

export default {
  name: 'app',
  data () {
    return {
      getShowLoading: true
    }
  },
  components: {
    Loader
  }
}
</script>

<style>

</style>
