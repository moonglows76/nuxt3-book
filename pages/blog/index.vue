<template>
  <div class="wrapper">
    <div class="container">
      <h1>Blog</h1>
      <p>エンジニアの日常生活をお届けします。</p>
      <div v-for="singleData in data" :key="singleData.id" class="blogCard">
        <div class="textsContainer">
          <h3>{{ singleData.title }}</h3>
          <p>{{ singleData.excerpt }}</p>
          <p>{{ singleData.date }}</p>
          <NuxtLink :to="singleData._path" class="linkButton">Read More</NuxtLink>
        </div>
        <div class="blogImg">
          <img :src="singleData.image" alt="blog-image">
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
  // useAsyncDataでmdファイルの中身を読み取る
  // "blogQuery"は処理の名前を指定
  // 処理の名前は他のファイルで使っていないものを指定する必要がある
  const { data } = await useAsyncData("blogQuery", () => 
    // idの数字が大きい順にソート
    queryContent("/blog").sort({ id: -1 }).find()
  )
</script>

<style scoped>

</style>