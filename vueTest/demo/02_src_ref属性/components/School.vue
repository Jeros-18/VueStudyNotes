<template>
    <div class="demo">
        <h2>学校名称：{{name}}</h2>
        <h2>学校地址：{{adress}}</h2>
        <button @click="showName">点我提示学校名称</button>
    </div>
</template>

<script>
export default {
    name:'School',
    data() {
        return {
            name:"安徽工程大学",
            adress:'芜湖市鸠江区'
        }
    },
    methods: {
        showName(){
            alert(this.name)
        }
    },
}
</script>

<style>
    .demo{
        background-color:blue;
    }
</style>