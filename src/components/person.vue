<template>
<div class="person">
    <h2>姓名：{{name}}</h2>
    <h2>年龄：{{age}}</h2>
    <button @click="changeName">修改名字</button>
    <button @click="changeAge">年龄+1</button>
    <button @click="showTel">点我查看联系方式</button>


</div>


</template>


<script lang="ts">
export default {
    name: "App",
    data() {
        return {
            name: "张三",
            age: 18,
            tel: "18552222222",
        }
    },
    methods: {
        changeName(){
            this.name="李四"
        },
        changeAge(){
            this.age=20
        },
        showTel(){
            alert(this.tel)
        }
    }




}




</script>


<style></style>