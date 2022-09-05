<template>
  <div class="bg-[#FFFFFF] relative xl:left-16 2xl:left-0">
    <section class="max-w-[1200px] mx-auto min-h-screen xl:flex gap-10">
      <NavbarVue navSelected="test" />
      <main class="flex-1">
        <AboutMainContentVue />
      </main>
    </section>
  </div>
</template>

<script>
import NavbarVue from "../components/pageDesigns/Navbar.vue"
import AboutMainContentVue from "../components/Page2/AboutMaincontent.vue"
export default {
  name: "TestView",
  components: {
    NavbarVue,

    AboutMainContentVue,
  },
}
</script>
