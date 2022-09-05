<template>
  <section
    class="min-h-[910px] py-10 px-5 xl:px-20 bg-[#F1F1F5] mt-10 rounded-[9px]"
  >
    <!-- heading  -->
    <h2
      class="poppins-font font-bold text-[#171724] text-xl lg:text-3xl pt-6 pb-16"
    >
      Recommended For You
    </h2>
    <div class="grid justify-center grid-col-1 md:grid-cols-2 gap-12">
      <!-- card wrapper  -->
      <div class="bg-transparent">
        <div
          class="relative before:absolute before:w-full before:h-full before:top-0 before:left-0 before:bg-gradient-to-b before:from-[rgba(255,255,255,_0)_3.7%] before:to-white w-full xl w-full:xl:w-[285px] h-[310px]"
        >
          <img
            src="../../assets/cards/card-1.png"
            alt=""
            class="w-full h-full object-cover"
          />
          <!-- sticker  -->
          <img
            src="../../assets/stickers/StarterBanner.svg"
            alt="starter"
            class="absolute top-4 left-0"
          />
          <div
            class="absolute top-0 left-0 w-full h-full flex items-end px-5 py-8"
          >
            <h3 class="popins-font font-bold text-[#171724] text-lg lg:text-xl">
              Building the Group
            </h3>
          </div>
        </div>
      </div>

      <!-- card #2  -->
      <div class="bg-transparent">
        <div
          class="relative before:absolute before:w-full before:h-full before:top-0 before:left-0 before:bg-gradient-to-b before:from-[rgba(255,255,255,_0)_3.7%] before:to-white w-full xl:w-[285px] h-[310px]"
        >
          <img
            src="../../assets/cards/card-2.png"
            alt=""
            class="w-full h-full object-cover"
          />
          <!-- sticker  -->
          <img
            src="../../assets/stickers/JerryMcQuireBanner.svg"
            alt="starter"
            class="absolute top-4 left-0"
          />
          <div
            class="absolute top-0 left-0 w-full h-full flex items-end px-5 py-8"
          >
            <h3 class="popins-font font-bold text-[#171724] text-lg lg:text-xl">
              Engagement In Your Group
            </h3>
          </div>
        </div>
      </div>

      <div class="bg-transparent">
        <div
          class="relative before:absolute before:w-full before:h-full before:top-0 before:left-0 before:bg-gradient-to-b before:from-[rgba(255,255,255,_0)_3.7%] before:to-white w-full xl:w-[285px] h-[310px]"
        >
          <img
            src="../../assets/cards/card-3.png"
            alt=""
            class="w-full h-full object-cover"
          />
          <!-- sticker  -->
          <img
            src="../../assets/stickers/ProfitFinderBanner.svg"
            alt="starter"
            class="absolute top-4 left-0"
          />
          <div
            class="absolute top-0 left-0 w-full h-full flex items-end px-5 py-8"
          >
            <h3 class="popins-font font-bold text-[#171724] text-lg lg:text-xl">
              Monetize Your Group
            </h3>
          </div>
        </div>
      </div>

      <div class="bg-transparent">
        <div
          class="relative before:absolute before:w-full before:h-full before:top-0 before:left-0 before:bg-gradient-to-b before:from-[rgba(255,255,255,_0)_3.7%] before:to-white w-full xl:w-[285px] h-[310px]"
        >
          <img
            src="../../assets/cards/card-4.png"
            alt=""
            class="w-full h-full object-cover"
          />
          <!-- sticker  -->
          <img
            src="../../assets/stickers/OpportunistBanner.svg"
            alt="starter"
            class="absolute top-4 left-0"
          />
          <div
            class="absolute top-0 left-0 w-full h-full flex items-end px-5 py-8"
          >
            <h3 class="popins-font font-bold text-[#171724] text-lg lg:text-xl">
              CTA Bootcamp - Live Series
            </h3>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "RecommendedVue",
}
</script>

<style></style>
