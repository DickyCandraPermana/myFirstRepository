<script setup>
import MainNavbar from './components/MainNavbar.vue'
import ContentArtikel from './components/ContentArtikel.vue'
import ContentGalery from './components/ContentGalery.vue'
import ContentKerjasama from './components/ContentKerjasama.vue'
import ContentBlog from './components/ContentBlog.vue'
import ContentAboutUs from './components/ContentAboutUs.vue'
import ContentCeritaSukses from './components/ContentCeritaSukses.vue'
import ContentGabung from './components/ContentGabung.vue'
import MainFooter from './components/MainFooter.vue'
</script>

<template>
  <MainNavbar />

  <main>
    <section class="header">
      <ContentArtikel />
      <ContentGalery />
    </section>
    <section>
      <ContentKerjasama />
    </section>
    <section>
      <ContentBlog />
    </section>
    <section>
      <ContentAboutUs />
    </section>
    <section>
      <ContentCeritaSukses />
    </section>
    <section>
      <ContentGabung />
    </section>
  </main>

  <MainFooter />
</template>

<style scoped>
.header {
  gap: 100px
}

header {
  width: 100%;
  height: 80px;
  display: flex;
  align-items: center;
  justify-content: space-around;
  border-bottom: 0.5px solid black;
  margin-bottom: 70px;
}

main {
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  align-items: center;
  gap: 50px;
  margin-bottom: 50px;
}

section {
  width: 80%;
  display: flex;
  justify-content: space-around;
}
</style>
