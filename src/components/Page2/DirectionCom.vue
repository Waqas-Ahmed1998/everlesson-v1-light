<template>
  <section class="px-10 pb-10 bg-[#F1F1F5]">
    <div class="w-full flex flex-col lg:flex-row py-4 lg:py-12 gap-4">
      <span
        class="roboto-font font-light 2xl md:3xl lg:text-4xl xl:text-5xl text-[#959CA0] text-center"
        >01</span
      >
      <!-- article content  -->
      <div class="text-center lg:text-left flex">
        <div>
          <h2
            class="popins-font font-bold text-lg md:text-xl lg:text-[26.6px] lg:leading-[39px] text-[#1C1E21]"
          >
            Directions
          </h2>
          <p
            class="roboto-font font-light text-sm leading-[24px] lg:pr-16 text-[#696973] pt-3"
          >
            Your first goal! This is your chance to receive your first badge.
            All you have to do is load your profile picture.Once you have
            updated your profile tell me how excited you are to create your
            audience and build up a tribe of hot raging fans. I also want to
            know that you are 110% commited to your success and will show up for
            each and every session.
          </p>
        </div>
        <img src="../../assets/banners/StarterBadgeLg.svg" alt="" class="" />
      </div>
    </div>
    <!-- request badge image and button wrapper  -->
    <section class="pr-10">
      <div class="flex items-center w-full gap-4 md:gap-6 xl:gap-10">
        <img
          src="https://media.istockphoto.com/photos/shot-of-a-young-businessman-using-a-laptop-in-a-modern-office-picture-id1354898581?b=1&k=20&m=1354898581&s=170667a&w=0&h=Jkv4uO6gEaLFtz6F22ZrEk4VQljqLNKMuVpdRlIYoEY="
          alt=""
          class="w-16 h-16 object-cover rounded-full"
        />
        <!-- chat box  -->
        <div class="relative w-full bg-white pt-3">
          <!-- chat pointer  -->
          <div
            class="absolute w-5 h-5 rotate-45 top-[50%] translate-y-[-50%] z-[0] bg-white -left-2"
          ></div>
          <textarea
            name=""
            placeholder="How excited are you?"
            id=""
            cols="30"
            rows="3"
            class="roboto-font bg-white w-full px-4 relative z-[2] outline-none overflow-y-hidden [resize:none] h-full text-sm text-[#696973]"
          ></textarea>
        </div>
      </div>
      <div class="flex items-center justify-end mt-10">
        <button
          class="w-fit roboto-font font-medium text-base rounded flex items-center justify-center py-4 bg-transparent border border-[#0062FF] shadow-[0px_2px_6px_rgba(0,0,0,_0.12)] text-[#0062FF] px-12 [@media(hover:hover)]:hover:bg-[#E5E5EE] transition-colors ease-in-out duration-150"
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
