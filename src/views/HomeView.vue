<template>
  <div class="bg-[#FFFFFF] xl:relative xl:left-16 2xl:left-0">
    <section
      class="max-w-[1200px] xl:mx-auto min-h-screen xl:flex xl:gap-10 px-0 xl:px-auto"
    >
      <NavbarVue navSelected="home" />
      <main class="xl:flex-1">
        <MainContentVue />
      </main>
    </section>
  </div>
</template>

<script>
import NavbarVue from "../components/pageDesigns/Navbar.vue"
import RecentActivityVue from "../components/pageDesigns/Sidebars/RecentActivity.vue"
import MainContentVue from "../components/pageDesigns/MainContent.vue"
export default {
  components: {
    NavbarVue,
    RecentActivityVue,
    MainContentVue,
  },
}
</script>
