<template>
  <section id="videoContent" class="max-w-full bg-[#F1F1F5]">
    <!-- video container  -->
    <div class="w-full">
      <!-- video wrapper  -->
      <div class="flex w-full aspect-auto min-h-[200px] md:min-h-[443px]">
        <iframe
          class="w-full min-h-full"
          src="https://www.youtube.com/embed/0mm57rH1sTE"
          title="YouTube video player"
          frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
          allowfullscreen
        ></iframe>
      </div>
      <section class="px-4 xl:px-10 py-5">
        <!-- video heading and icons  -->
        <div class="space-y-1 flex justify-between items-center">
          <h2
            class="popins-font text-base md:text-lg lg:text-2xl xl:text-[34px] xl:leading-[52px] font-bold text-[#1C1E21]"
          >
            Load Your Profile Picture
          </h2>
          <!-- icons container  -->
          <div class="flex gap-8 items-center">
            <!-- bookmark icon  -->
            <i class="cursor-pointer"
              ><svg
                class="w-[18px] h-[18px] lg:w-[23px] lg:h-[23px]"
                width="19"
                height="23"
                viewBox="0 0 19 23"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M5.47632 7.82599H1.73633C1.65451 7.82599 1.57345 7.80987 1.49786 7.77856C1.42228 7.74726 1.35363 7.70141 1.29578 7.64355C1.23793 7.5857 1.19201 7.51699 1.16071 7.44141C1.1294 7.36582 1.11328 7.28482 1.11328 7.203V3.46301C1.11328 3.13563 1.17782 2.81144 1.3031 2.50897C1.42839 2.20651 1.61201 1.93169 1.84351 1.7002C2.075 1.4687 2.34982 1.28508 2.65228 1.15979C2.95475 1.03451 3.27894 0.969971 3.60632 0.969971H15.4473C15.7747 0.969971 16.0988 1.03451 16.4013 1.15979C16.7038 1.28508 16.9786 1.4687 17.2101 1.7002C17.4416 1.93169 17.6253 2.20651 17.7505 2.50897C17.8758 2.81144 17.9403 3.13563 17.9403 3.46301V20.863C17.9404 20.9803 17.9073 21.0954 17.8448 21.1948C17.7824 21.2941 17.6932 21.3739 17.5875 21.4247C17.4817 21.4756 17.3637 21.4956 17.2471 21.4824C17.1305 21.4692 17.02 21.4233 16.9283 21.35L12.0973 17.486C11.9869 17.3977 11.8497 17.3496 11.7083 17.3496C11.5669 17.3496 11.4297 17.3977 11.3193 17.486L6.48828 21.35C6.39661 21.4233 6.28611 21.4692 6.16949 21.4824C6.05288 21.4956 5.93492 21.4756 5.82916 21.4247C5.72341 21.3739 5.63414 21.2941 5.57172 21.1948C5.50929 21.0954 5.47625 20.9803 5.47632 20.863V2.84003C5.47632 2.34407 5.27928 1.86839 4.92859 1.5177C4.5779 1.16701 4.10228 0.969971 3.60632 0.969971"
                  stroke="#92929C"
                  stroke-width="1.197"
                  stroke-linejoin="round"
                />
              </svg>
            </i>
            <!-- share icon  -->
            <i class="cursor-pointer"
              ><svg
                class="w-[18px] h-[18px] lg:w-[23px] lg:h-[23px]"
                width="23"
                height="23"
                viewBox="0 0 23 23"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M4.7277 15.3341C6.7104 15.3341 8.3177 13.7268 8.3177 11.7441C8.3177 9.76135 6.7104 8.15405 4.7277 8.15405C2.74499 8.15405 1.1377 9.76135 1.1377 11.7441C1.1377 13.7268 2.74499 15.3341 4.7277 15.3341Z"
                  stroke="#92929C"
                  stroke-width="1.197"
                  stroke-linejoin="round"
                />
                <path
                  d="M17.8898 8.753C19.8725 8.753 21.4798 7.1457 21.4798 5.163C21.4798 3.1803 19.8725 1.573 17.8898 1.573C15.9071 1.573 14.2998 3.1803 14.2998 5.163C14.2998 7.1457 15.9071 8.753 17.8898 8.753Z"
                  stroke="#92929C"
                  stroke-width="1.197"
                  stroke-linejoin="round"
                />
                <path
                  d="M17.8898 21.9149C19.8725 21.9149 21.4798 20.3076 21.4798 18.3249C21.4798 16.3422 19.8725 14.7349 17.8898 14.7349C15.9071 14.7349 14.2998 16.3422 14.2998 18.3249C14.2998 20.3076 15.9071 21.9149 17.8898 21.9149Z"
                  stroke="#92929C"
                  stroke-width="1.197"
                  stroke-linejoin="round"
                />
                <path
                  d="M8.31641 13.5381L14.2994 16.5291"
                  stroke="#92929C"
                  stroke-width="1.197"
                  stroke-linejoin="round"
                />
                <path
                  d="M14.2994 6.95703L8.31641 9.94803"
                  stroke="#92929C"
                  stroke-width="1.197"
                  stroke-linejoin="round"
                />
              </svg>
            </i>
          </div>
        </div>
        <!-- video watch details and user pictures  -->
        <div class="flex items-center gap-6 py-4">
          <!-- image wrapper  -->
          <div class="flex items-center gap-2">
            <img
              src="../../assets/video/perrySmall.png"
              alt="perry"
              class="rounded-full w-[27px] h-[27px] object-cover"
            />

            <img
              src="../../assets/video/chadSmall.png"
              alt="chad"
              class="rounded-full w-[27px] h-[27px] object-cover"
            />
          </div>
          <span
            class="roboto-font font-light text-[#696973] gap-2 text-xs lg:text-sm flex items-center"
            >Perry Belcher & Chad Nicely</span
          >

          <span
            class="roboto-font font-light text-[#696973] gap-2 text-xs lg:text-sm flex items-center"
            ><i
              ><svg
                width="22"
                height="15"
                viewBox="0 0 22 15"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M11.2276 13.8168C16.8438 13.8168 21.3966 10.8722 21.3966 7.23984C21.3966 3.60747 16.8438 0.662842 11.2276 0.662842C5.61141 0.662842 1.05859 3.60747 1.05859 7.23984C1.05859 10.8722 5.61141 13.8168 11.2276 13.8168Z"
                  stroke="#92929C"
                  stroke-width="1.196"
                  stroke-linejoin="round"
                />
                <path
                  d="M11.2276 10.8279C13.2092 10.8279 14.8156 9.22145 14.8156 7.23986C14.8156 5.25826 13.2092 3.65186 11.2276 3.65186C9.24605 3.65186 7.63965 5.25826 7.63965 7.23986C7.63965 9.22145 9.24605 10.8279 11.2276 10.8279Z"
                  stroke="#92929C"
                  stroke-width="1.196"
                  stroke-miterlimit="10"
                />
              </svg> </i
            >345 people have watched this</span
          >
        </div>
      </section>
    </div>
  </section>
</template>

<script>
export default {
  name: "TestVideoVue",
}
</script>

<style></style>
