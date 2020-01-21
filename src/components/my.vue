<template>
  <div class="hello">
    <h1 @click="showLog">{{ msg }}</h1>
    <p>
      test for vlogv ...
    </p>
  </div>
</template>

<script>
import Vue from 'vue'
import vlogv from '../libs/index'
// this.$log.log('show markbye')

Vue.use(vlogv, { prefix: new Date().getFullYear() + '-' + (parseInt(new Date().getMonth() + 1)) + '-' + new Date().getDate(), dev: true })

export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  methods: {
    showLog () {
      this.$log.log('show markbye')
      this.$log.warn('show warn')
      this.$log.debug('show warn')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
