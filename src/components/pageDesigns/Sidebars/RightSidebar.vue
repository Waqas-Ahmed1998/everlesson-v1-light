<template>
  <aside class="block lg:basis-[390px] space-y-8 my-10 xl:my-0">
    <main class="bg-[#F1F1F5] px-9 rounded-[9px] py-11">
      <!-- membership  -->
      <section id="membership" class="pb-6 border-b border-[#D5D5DC]">
        <!-- image container  -->
        <div class="w-full flex gap-5 pb-5">
          <img
            src="../../../assets/sidebar/PerryBelcher.png"
            alt=""
            class="w-[70px] h-[70px] rounded-full object-cover bg-center"
          />
          <img
            src="../../../assets/sidebar/ChadNicely.png"
            alt=""
            class="rounded-full w-[70px] h-[70px] object-contain bg-center"
          />
        </div>
        <h2
          class="popins-font text-[#1C1E21] font-bold text-lg xl:text-2xl pb-4"
        >
          About Membership
        </h2>
        <p
          class="roboto-font font-light text-base xl:text-[18.45px] lg:leading-8 text-[#696973]"
        >
          Welcome to the membership for "Platform Founders." It is here that you
          will find the line of TOP QUALITY products that both Perry Belcher and
          Chad Nicely have produced to help your business reach new heights.
        </p>
      </section>
      <!-- access section  -->
      <section class="mt-4">
        <h2
          class="roboto-font font-bold text-base xl:text-lg text-[#1C1E21] text-center my-7"
        >
          Access to all lessons <br />
          for $/month (billed annually)
        </h2>
        <!-- button wrapper  -->
        <div class="w-full space-y-4">
          <button
            class="roboto-font font-medium text-base xl:text-lg w-full rounded flex items-center justify-center py-3 bg-[#0062FF] shadow-[0px_2px_6px_rgba(0,0,0,_0.12)] text-white"
          >
            GET STARTED
          </button>
          <button
            class="roboto-font font-medium text-base xl:text-lg w-full rounded flex items-center justify-center py-3 bg-transparent border border-[#0062FF] shadow-[0px_2px_6px_rgba(0,0,0,_0.12)] text-[#0062FF]"
          >
            LEARN MORE
          </button>
        </div>
      </section>
    </main>
    <RecentActivityVue />
  </aside>
</template>

<script>
import RecentActivityVue from "./RecentActivity.vue"
export default {
  name: "RightSidebarVue",
  components: {
    RecentActivityVue,
  },
}
</script>

<style></style>
