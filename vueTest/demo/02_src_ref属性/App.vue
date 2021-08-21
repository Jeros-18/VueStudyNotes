<template>
  <div id="app">
   
    <h1 v-text='msg' ref="title"></h1></h1>
    <button ref="btn" @click="showDOM">点我输出上方DOM元素</button>
    <School ref="sch"></School>
    
    
  </div>
</template>

<script>
import School from './components/School.vue'


export default {
  name: 'App',
  components: {
    School,
  },
  data() {
    return {
      msg:'hello',
    }
  
  },

  methods: {
    showDOM(){
      console.log(this.$refs.title)
      console.log(this.$refs.btn)
      console.log(this.$refs.sch)
    }
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
