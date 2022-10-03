<template>
  <div>
    <div class="hero">
      <img :src="data.image" alt="blog-image">
    </div>
    <div class="wrapper">
      <div class="container">
        <h1>{{ data.title }}</h1>
        <p>{{ data.date }}</p>
        <ContentDoc />
      </div>
    </div>
  </div>
</template>

<script setup>
  // useAsyncDataでmdファイルの中身を読み取る
  // useRoute().pathは現在のURLを処理の名前として指定
  // 処理の名前は他のファイルで使っていないものを指定する必要がある
  const { data } = await useAsyncData(useRoute().path, () => 
    // useRoute().pathで現在のURLを取得して、queryContentに渡す
    // findOneでデータを1つだけ取得
    queryContent(useRoute().path).findOne()
  )

</script>

<style scoped>

</style>