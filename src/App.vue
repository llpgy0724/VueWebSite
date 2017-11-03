<template>
  <div id="app">
    <fixedbg></fixedbg>
  </div>
</template>

<script>
//import loader from './components/common/loader/loader'
import fixedbg from './components/common/fixedbg/fixedbg'
export default {
  name: 'app',
  data () {
    return {
      getShowLoading: true
    }
  },
  components: {
    //loader
    fixedbg
  }
}
</script>

<style>

</style>
