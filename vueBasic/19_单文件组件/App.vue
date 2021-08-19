<template>
   <div>
      <School></School>
      <Student></Student>
   </div>
</template>

<script>
import School from '../../codes/vue_basic/19_单文件组件/School.vue'
import Student from '../../codes/vue_basic/19_单文件组件/Student.vue'
export default {
  components: { School, Student },
   name:'App',


}
</script>

<style>

</style>