<template>
  <section id="mainContent" class="px-0 pt-10 lg:py-10 lg:space-y-10">
    <!-- sidebard and middle content container  -->
    <section
      class="flex flex-col xl:flex-row w-full xl:gap-7 xl:justify-end 2xl:justify-center px-6"
    >
      <!-- middle content container  -->
      <div
        class="flex flex-col xl:max-w-[780px] lg:bg-[#F1F1F5] rounded-[9px] px-0 lg:px-16 lg:py-11"
      >
        <VideoContentVue />

        <ArticlesVue />
      </div>
      <RightSidebarVue />
    </section>
    <div class="px-4 lg:px-0">
      <AccesVue />
    </div>
    <FooterVue />
  </section>
</template>

<script>
import VideoContentVue from "./VideoContent.vue"
import AboutProductVue from "./AboutProduct.vue"
import RightSidebarVue from "./Sidebars/RightSidebar.vue"
import ArticlesVue from "./Article.vue"
import AccesVue from "./Acces.vue"
import FooterVue from "./Footer.vue"
export default {
  name: "MainContent",
  components: {
    VideoContentVue,
    AboutProductVue,
    RightSidebarVue,
    ArticlesVue,
    AccesVue,
    FooterVue,
  },
}
</script>

<style></style>
