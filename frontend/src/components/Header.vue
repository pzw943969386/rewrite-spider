<script setup lang="ts">
import { useRouter } from 'vue-router'

const router = useRouter()

const goArticle = () => {
  router.push('/article')
}

const goHome = () => {
  router.push('/')
}

const goSplite = () => {
  router.push('/splite')
}

const goGetContent = () => {
  router.push('/get_content')
}

const goWrite = () => {
  router.push('/write')
}
</script>

<template>
  <div class="container">
    <div class="header">
      <div @click="goHome">首页</div>
      <div @click="goArticle">文章列表</div>
      <div @click="goSplite">断句</div>
      <div @click="goGetContent">获取内容</div>
      <div @click="goWrite">写作</div>
    </div>
  </div>
</template>

<style scoped lang="less">
.container {
  width: 100%;
  height: 100%;
  padding-top: 50px;
}
.header {
  width: 100%;
  height: 50px;
  background-color: #000;
  display: flex;
  align-items: center;
  position: fixed;
  top: 0;
  left: 0;
  z-index: 1000;
  div {
    width: 100px;
    color: #fff;
    font-size: 16px;
    font-weight: bold;
    cursor: pointer;
    text-align: center;
  }
}
</style>
