<template>
  <div>
    <div class="hero">
      <img src="~/assets/images/index-hero.jpg" alt="hero">
      <div class="textContainer">
        <h1>I'm Abe Hiroki!</h1>
        <h3>JavaScript Developer</h3>
      </div>
    </div>
    <div class="container">
      <div class="profile">
        <div>
          <h2>JavaScriptNerd</h2>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quis quibusdam ex veritatis laborum enim sequi eaque sed quia incidunt repellat laudantium accusamus, quod itaque eligendi nisi, in aliquid debitis atque.</p>
        </div>
        <img src="~/assets/images/profile.jpg" alt="profile">
      </div>
      <div class="skills">
        <h2>Skills</h2>
        <div class="skillsContainer">
          <div>
            <img src="~/assets/images/javascript.svg" alt="javascript">
            <span>JavaScript/10years</span>
          </div>
          <div>
            <img src="~/assets/images/react.svg" alt="react">
            <span>React/4years</span>
          </div>
          <div>
            <img src="~/assets/images/vue.svg" alt="vue">
            <span>Vue/4years</span>
          </div>
          <div>
            <img src="~/assets/images/nuxt.svg" alt="nuxt">
            <span>Nuxt/3years</span>
          </div>
        </div>
      </div>
      <div class="ctaButton">
        <NuxtLink to="/contact">Make It Happen!</NuxtLink>
      </div>
    </div>
  </div>
</template>

<script setup>

</script>

<style scoped>

</style>