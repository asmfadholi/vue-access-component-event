<template>  
  <div>
      <vue-clockpicker :value="searchText" @timeset="searchText = $event" />
    <h1>{{ searchText }}</h1>
  </div>
</template>

<script>
import VueClockPicker from '@pencilpix/vue2-clock-picker';
import '@pencilpix/vue2-clock-picker/dist/vue2-clock-picker.min.css';

export default {
  name: 'HelloWorld',
  components: {
    'vue-clockpicker': VueClockPicker,
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      searchText: '20:00',
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
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
