<template>
  <div>
    <Header />
    <main>
      <!-- app.vueが土台になって、layouts/default.vueはその次のレベルの土台になる -->
      <!-- pagesフォルダ内をslotで読み込む -->
      <slot />
    </main>
    <Footer />
  </div>
</template>