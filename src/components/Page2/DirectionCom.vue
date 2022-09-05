<template>
  <section class="lg:px-5 xl:px-10 pb-10 bg-[#F1F1F5]">
    <div class="w-full flex flex-row py-4 px-2 lg:px-0 lg:py-12 gap-4">
      <span
        class="roboto-font font-light text-2xl lg:text-4xl xl:text-5xl text-[#959CA0] text-center"
        >01</span
      >
      <!-- article content  -->
      <div class="items-center text-left flex">
        <div>
          <h2
            class="popins-font font-bold text-lg md:text-xl lg:text-[26.6px] lg:leading-[39px] text-[#1C1E21]"
          >
            Directions
          </h2>
          <p
            class="roboto-font font-light text-xs lg:text-sm leading-[24px] pr-5 lg:pr-10 xl:pr-16 text-[#696973] pt-3"
          >
            Your first goal! This is your chance to receive your first badge.
            All you have to do is load your profile picture.Once you have
            updated your profile tell me how excited you are to create your
            audience and build up a tribe of hot raging fans. I also want to
            know that you are 110% commited to your success and will show up for
            each and every session.
          </p>
        </div>
        <img
          src="../../assets/banners/StarterBadgeLg.svg"
          alt=""
          class="w-20 h-20 lg:h-28 lg:w-28 xl:w-30 xl:h-30"
        />
      </div>
    </div>
    <!-- request badge image and button wrapper  -->
    <section class="px-3 lg:px-0 lg:pr-5 xl:pr-10 mt-5 lg:mt-2 xl:mt-0">
      <div class="flex items-center w-full gap-4 md:gap-6 xl:gap-10">
        <img
          src="https://media.istockphoto.com/photos/shot-of-a-young-businessman-using-a-laptop-in-a-modern-office-picture-id1354898581?b=1&k=20&m=1354898581&s=170667a&w=0&h=Jkv4uO6gEaLFtz6F22ZrEk4VQljqLNKMuVpdRlIYoEY="
          alt=""
          class="w-14 h-14 lg:w-16 lg:h-16 object-cover rounded-full"
        />
        <!-- chat box  -->
        <div class="relative w-full bg-white pt-3">
          <!-- chat pointer  -->
          <div
            class="absolute w-3 h-3 lg:w-5 lg:h-5 rotate-45 top-[50%] translate-y-[-50%] z-[0] bg-white -left-2"
          ></div>
          <textarea
            name=""
            placeholder="How excited are you?"
            id=""
            cols="30"
            rows="3"
            class="roboto-font bg-white w-full px-4 relative z-[2] outline-none overflow-y-hidden [resize:none] h-full text-xs lg:text-sm text-[#696973]"
          ></textarea>
        </div>
      </div>
      <div class="flex items-center justify-end mt-10">
        <button
          class="w-full lg:w-fit roboto-font font-medium text-base rounded flex items-center justify-center bg-transparent border border-[#0062FF] shadow-[0px_2px_6px_rgba(0,0,0,_0.12)] text-[#0062FF] py-4 px-6 lg:py-4 lg:px-12 [@media(hover:hover)]:hover:bg-[#E5E5EE] transition-colors ease-in-out duration-150"
        >
          REQUEST YOUR BADGE
        </button>
      </div>
    </section>
  </section>
</template>

<script>
export default {
  name: "DirectionsComVue",
}
</script>

<style></style>
