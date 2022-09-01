<template>
  <section id="mainContent" class="px-2 py-10 space-y-10">
    <!-- sidebard and middle content container  -->
    <section class="flex w-full gap-7 xl:justify-end 2xl:justify-center">
      <!-- middle content container  -->
      <div class="flex flex-col max-w-[780px] rounded-[9px] h-fit">
        <TestVideoVue />
        <DirecionsNav />
        <DirectionsComVue />
        <RecommendedVue />
      </div>
      <RightSidebarVue />
    </section>

    <AccesVue />
    <FooterVue />
  </section>
</template>

<script>
import RecommendedVue from "./Recommended.vue"
import RightSidebarVue from "../pageDesigns/Sidebars/RightSidebar.vue"
import DirecionsNav from "./DirectionsNav.vue"
import DirectionsComVue from "./DirectionCom.vue"
import AccesVue from "../pageDesigns/Acces.vue"
import FooterVue from "../pageDesigns/Footer.vue"
import TestVideoVue from "./TestVideo.vue"
export default {
  name: "AboutMainContentVue",
  components: {
    RightSidebarVue,
    RecommendedVue,
    AccesVue,
    FooterVue,
    TestVideoVue,
    DirecionsNav,
    DirectionsComVue,
  },
}
</script>

<style></style>
