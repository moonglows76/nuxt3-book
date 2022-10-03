<template>
  <footer>
    <div class="insideContainer">
      <a href="https://www.google.com"><img src="~/assets/images/github.svg" alt=""></a>
      <a href="https://www.google.com"><img src="~/assets/images/linkedin.svg" alt=""></a>
      <a href="https://www.google.com"><img src="~/assets/images/twitter.svg" alt=""></a>
      <a href="https://www.google.com"><img src="~/assets/images/facebook.svg" alt=""></a>
      <hr>
      <NuxtLink to="/blog">Blog</NuxtLink>
      <NuxtLink to="/contact">Contact</NuxtLink>
      <p>©{{ new Date().getFullYear() }} Abe Hiroki</p>
    </div>
  </footer>
</template>