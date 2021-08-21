<template>
  <div>
      <h2 @click="showName">学校名称：{{name}}</h2></h2>
      <h2>学校地址：{{adress}}</h2>
  </div>
</template>

<script>
 import {hunhe} from '../mixin'

export default {
   
    name:'School',
    data() {
        return {
            name:'安徽工程大学',
            adress:'安徽省芜湖市'
        }
    },

    mixins:[hunhe]
}
</script>

<style>

</style>