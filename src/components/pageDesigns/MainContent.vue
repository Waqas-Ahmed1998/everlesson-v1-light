<template>
  <section id="mainContent" class="px-2 py-10 space-y-10">
    <!-- sidebard and middle content container  -->
    <section class="flex w-full gap-7 xl:justify-end 2xl:justify-center">
      <!-- middle content container  -->
      <div
        class="flex flex-col max-w-[780px] bg-[#F1F1F5] rounded-[9px] px-16 py-11"
      >
        <VideoContentVue />

        <ArticlesVue />
      </div>
      <RightSidebarVue />
    </section>
    <AccesVue />
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
