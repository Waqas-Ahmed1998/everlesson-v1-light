<template>
  <div class="bg-[#FFFFFF] relative xl:left-16 2xl:left-0">
    <section class="max-w-[1200px] mx-auto min-h-screen flex gap-10">
      <NavbarVue navSelected="home" />
      <main class="flex-1">
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
