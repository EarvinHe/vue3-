<template>
  <!-- Vue3的app组件可以没有根标签 -->
 <h1>一个人的信息:</h1>
 <h2>姓名:{{ name }}</h2>
 <h2>年龄:{{ age }}</h2>
 <button @click="readUser">点击</button>
</template>

<script>


export default {
  name: 'App',
  setup() {
    let name ='张三'
    let age = '18'

    // 方法
    function readUser(){
      alert(`我叫${name},今年${age}`)
    }

    // 必须有返回值
    return{
      name,age,readUser
    }
  }
}
</script>

<style>

</style>
