<template>
    <div class="demo">
        <h2>学生姓名：{{name}}</h2>
        <h2>学生性别：{{sex}}</h2>
        <h2>学生年龄：{{myAge+1}}</h2>
        <button @click="updateAge">尝试修改收到的年龄</button>
    </div>
</template>

<script>
export default {
    name:'Student',
    data() {
        return {
            
            myAge:this.age
        }
    },
    methods: {
        updateAge(){
            this.myAge++
        }
    },
    props:{
        name:String,
        age:Number,
        sex:String
    }
}
</script>

<style>
    .demo{
        background-color:blue;
    }
</style>