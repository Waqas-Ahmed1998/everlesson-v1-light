<template>
  <!-- wrapper  -->
  <div class="">
    <!-- mobile burger manue  -->
    <div
      class="w-full flex lg:hidden items-center justify-between px-5 pt-8 pb-5"
    >
      <span
        class="helvetica-font bg-[#F1F1F5] text-[24.17px] w-[35.33px] h-[35.33px] rounded-full p-1 text-[#92929C] flex items-center justify-center"
      >
        E
      </span>
      <!-- burger icon  -->
      <span
        @click="mobileBurgerManue = !mobileBurgerManue"
        :class="`cursor-pointer relative z-[202]  ${
          mobileBurgerManue
            ? 'opacity-[0] pointer-events-none'
            : 'opacity-[1] pointer-events-auto '
        }`"
      >
        <i
          ><svg
            width="40"
            height="40"
            viewBox="0 0 40 40"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M11 14H29"
              stroke="#92929C"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
            <path
              d="M11 20H29"
              stroke="#92929C"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
            <path
              d="M11 26H29"
              stroke="#92929C"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
          </svg>
        </i>
      </span>
    </div>
    <nav
      :class="`  min-h-screen xl:flex  justify-between fixed top-0 lg:top-auto left-0 lg:left-2  z-[200]   ${
        sideNavCollapse ? 'border-r' : 'border-none'
      }`"
    >
      <!-- nav links wrapper  -->
      <div
        :class="` transition-opacity lg:opacity-[1] z-[-1]  lg:w-fit   bg-black/50  relative    ${
          mobileBurgerManue
            ? '  ease-out  duration-200 opacity-[1] w-[100vw]   '
            : '  duration-300 opacity-[0]   w-0'
        }`"
      >
        <!-- mobile nav close icon  -->
        <i
          @click="mobileBurgerManue = false"
          :class="`absolute inline-block top-8 right-5 z-[220] lg:hidden transition-all ${
            mobileBurgerManue
              ? ' translate-x-[0%] duration-300 ease-out'
              : '-translate-x-[1200%] duration-200 ease-in  '
          }`"
        >
          <svg
            width="34"
            height="35"
            viewBox="0 0 34 35"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M17.4704 33.942C8.37372 33.942 0.999405 26.5677 0.999405 17.471C0.999405 8.37432 8.37372 1 17.4704 1C26.5671 1 33.9414 8.37432 33.9414 17.471C33.9414 26.5677 26.5671 33.942 17.4704 33.942Z"
              fill="white"
              stroke="#D5D5DC"
              stroke-width="0.5"
              stroke-miterlimit="10"
            />
            <path
              d="M18.8571 24.9729L12.5381 18.2859C12.3323 18.064 12.2179 17.7726 12.2179 17.4699C12.2179 17.1673 12.3323 16.8758 12.5381 16.6539L18.8571 9.96893C18.9555 9.8624 19.0749 9.7774 19.2077 9.71926C19.3406 9.66112 19.484 9.6311 19.6291 9.6311C19.7741 9.6311 19.9175 9.66112 20.0504 9.71926C20.1833 9.7774 20.3026 9.8624 20.401 9.96893C20.6071 10.1909 20.7217 10.4826 20.7217 10.7854C20.7217 11.0883 20.6071 11.38 20.401 11.6019L14.854 17.4709L20.4021 23.3409C20.6081 23.5629 20.7227 23.8546 20.7227 24.1574C20.7227 24.4603 20.6081 24.752 20.4021 24.9739C20.3036 25.0807 20.1842 25.1659 20.0512 25.2241C19.9182 25.2823 19.7745 25.3124 19.6293 25.3123C19.4841 25.3122 19.3405 25.282 19.2076 25.2236C19.0747 25.1652 18.9553 25.0798 18.8571 24.9729Z"
              fill="#B5B5BD"
            />
          </svg>
        </i>
        <!-- nav links   -->
        <section
          :class="`transition-transform   ${
            mobileBurgerManue
              ? ' -translate-x-[0]  ease-out  duration-200 z-[205]  px-2 '
              : ' -translate-x-[100%] lg:translate-x-0   ease-in-out duration-300  '
          } h-screen relative   bg-white flex  shadow-[2px_0_8px_#E7E7EE] lg:shadow-none rounded-[0px_18px_18px_0px] lg:rounded-none  lg:w-fit lg:px-2 flex-col justify-between   pb-10 pt-24 xl:py-12 xl:pb-0`"
        >
          <!-- logo  -->
          <span
            class="hidden helvetica-font bg-[#F1F1F5] text-[35.17px] w-[55.33px] h-[55.33px] rounded-full p-1 text-[#92929C] xl:flex items-center justify-center"
          >
            E
          </span>
          <!-- nav links  -->
          <div class="flex flex-col gap-6 w-full items-center">
            <!-- home icon  -->
            <router-link to="/">
              <i
                :class="`cursor-pointer block p-[8px]  xl:p-[10px] rounded-full transition-colors ease-in-out duration-150 [@media(hover:hover)]:hover:bg-[#F1F1F5] ${
                  navSelected == 'home' && 'bg-[#F1F1F5]'
                }`"
              >
                <svg
                  class="w-[24px] h-[24px] xl:w-[31px] xl:h-[31px]"
                  width="31"
                  height="31"
                  viewBox="0 0 31 35"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M29.3865 12.4641L17.2455 1.54008C16.8416 1.17696 16.3181 0.975246 15.7749 0.973401C15.2318 0.971557 14.7069 1.16971 14.3005 1.53007L1.97252 12.4631C1.73867 12.6705 1.55145 12.9252 1.42321 13.2103C1.29497 13.4954 1.22861 13.8045 1.22852 14.1171V31.3331C1.22852 31.6234 1.28571 31.9108 1.39684 32.179C1.50796 32.4472 1.67084 32.6909 1.87616 32.8961C2.08149 33.1014 2.32523 33.2641 2.59348 33.3751C2.86172 33.4861 3.14921 33.5432 3.43952 33.5431H10.9535C11.1234 33.5432 11.2915 33.5099 11.4485 33.4449C11.6054 33.38 11.748 33.2847 11.8681 33.1647C11.9882 33.0446 12.0834 32.902 12.1484 32.745C12.2133 32.5881 12.2466 32.4199 12.2465 32.2501V27.1831C12.2281 26.2815 12.5527 25.4067 13.1547 24.7354C13.7568 24.0641 14.5913 23.6465 15.4895 23.5671C15.9544 23.5422 16.4195 23.6123 16.8564 23.7731C17.2934 23.9339 17.693 24.182 18.0308 24.5023C18.3687 24.8226 18.6378 25.2084 18.8217 25.6361C19.0056 26.0638 19.1005 26.5245 19.1005 26.9901V32.2471C19.1004 32.4169 19.1337 32.5851 19.1987 32.742C19.2636 32.899 19.3588 33.0416 19.4789 33.1617C19.599 33.2818 19.7416 33.377 19.8985 33.4419C20.0555 33.5068 20.2237 33.5402 20.3935 33.5401H27.9075C28.1978 33.5402 28.4853 33.4831 28.7536 33.3721C29.0218 33.2611 29.2655 33.0984 29.4709 32.8931C29.6762 32.6879 29.8391 32.4442 29.9502 32.176C30.0613 31.9078 30.1185 31.6204 30.1185 31.3301V14.1071C30.1184 13.7972 30.0532 13.4908 29.9271 13.2078C29.801 12.9247 29.6168 12.6713 29.3865 12.4641V12.4641Z"
                    stroke="#92929C"
                    stroke-width="1.607"
                    stroke-miterlimit="10"
                  />
                </svg> </i
            ></router-link>

            <!-- paper icon  -->
            <router-link to="/test">
              <i
                :class="`cursor-pointer block p-[8px] xl:p-[10px] rounded-full transition-colors ease-in-out duration-150 [@media(hover:hover)]:hover:bg-[#F1F1F5] ${
                  navSelected == 'test' && 'bg-[#F1F1F5]'
                } `"
              >
                <svg
                  class="w-[24px] h-[24px] xl:w-[31px] xl:h-[31px]"
                  width="31"
                  height="31"
                  viewBox="0 0 27 35"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M24.934 1.33398H1.528C1.23639 1.33398 1 1.57038 1 1.86198V33.188C1 33.4796 1.23639 33.716 1.528 33.716H24.934C25.2256 33.716 25.462 33.4796 25.462 33.188V1.86198C25.462 1.57038 25.2256 1.33398 24.934 1.33398Z"
                    stroke="#92929C"
                    stroke-width="1.607"
                    stroke-miterlimit="10"
                  />
                  <path
                    d="M6.03223 9.66089H20.8352"
                    stroke="#92929C"
                    stroke-width="1.607"
                    stroke-miterlimit="10"
                    stroke-linecap="round"
                  />
                  <path
                    d="M6.03223 15.2129H20.8352"
                    stroke="#92929C"
                    stroke-width="1.607"
                    stroke-miterlimit="10"
                    stroke-linecap="round"
                  />
                  <path
                    d="M6.03223 20.7639H20.8352"
                    stroke="#92929C"
                    stroke-width="1.607"
                    stroke-miterlimit="10"
                    stroke-linecap="round"
                  />
                  <path
                    d="M15.2842 26.3149H20.8352"
                    stroke="#92929C"
                    stroke-width="1.607"
                    stroke-miterlimit="10"
                    stroke-linecap="round"
                  />
                </svg> </i
            ></router-link>

            <!-- folder icon  -->
            <i
              class="cursor-pointer block p-[8px] xl:p-[10px] rounded-full transition-colors ease-in-out duration-150 [@media(hover:hover)]:hover:bg-[#F1F1F5]"
            >
              <svg
                class="w-[24px] h-[24px] xl:w-[31px] xl:h-[31px]"
                width="31"
                height="31"
                viewBox="0 0 30 27"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M26.474 1.66797H3.202C1.98587 1.66797 1 2.65384 1 3.86997V23.188C1 24.4041 1.98587 25.39 3.202 25.39H26.474C27.6901 25.39 28.676 24.4041 28.676 23.188V3.86997C28.676 2.65384 27.6901 1.66797 26.474 1.66797Z"
                  stroke="#92929C"
                  stroke-width="1.607"
                  stroke-miterlimit="10"
                />
                <path
                  d="M1 8.00684H28.676"
                  stroke="#92929C"
                  stroke-width="1.607"
                  stroke-miterlimit="10"
                />
              </svg>
            </i>

            <!-- star icon  -->
            <i
              class="cursor-pointer block p-[8px] xl:p-[10px] rounded-full transition-colors ease-in-out duration-150 [@media(hover:hover)]:hover:bg-[#F1F1F5]"
            >
              <svg
                class="w-[24px] h-[24px] xl:w-[31px] xl:h-[31px]"
                width="31"
                height="31"
                viewBox="0 0 34 32"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M18.697 2.21912L21.88 8.66815C22.036 8.98419 22.2666 9.25753 22.5518 9.46466C22.8369 9.67179 23.1682 9.80648 23.517 9.85712L30.634 10.8911C31.0354 10.9494 31.4125 11.1189 31.7226 11.3804C32.0328 11.6418 32.2635 11.9848 32.3889 12.3706C32.5143 12.7564 32.5292 13.1695 32.432 13.5634C32.3349 13.9572 32.1294 14.316 31.839 14.5991L26.689 19.6191C26.4365 19.8651 26.2477 20.1687 26.1388 20.5039C26.0299 20.8391 26.0043 21.1958 26.064 21.5432L27.279 28.6321C27.3477 29.0319 27.3032 29.443 27.1504 29.8188C26.9976 30.1946 26.7427 30.5201 26.4145 30.7585C26.0863 30.997 25.6979 31.1387 25.2933 31.1678C24.8886 31.1969 24.4839 31.1122 24.125 30.9232L17.76 27.5771C17.4479 27.4131 17.1006 27.3273 16.748 27.3273C16.3954 27.3273 16.0481 27.4131 15.736 27.5771L9.371 30.9232C9.01205 31.1122 8.60737 31.1969 8.20274 31.1678C7.79812 31.1387 7.40972 30.997 7.0815 30.7585C6.75328 30.5201 6.49835 30.1946 6.34557 29.8188C6.19279 29.443 6.14825 29.0319 6.217 28.6321L7.432 21.5432C7.49148 21.1958 7.46567 20.8392 7.3568 20.504C7.24793 20.1689 7.05925 19.8652 6.807 19.6191L1.657 14.5991C1.36666 14.3163 1.16117 13.9579 1.06374 13.5645C0.966309 13.171 0.980814 12.7581 1.10562 12.3725C1.23042 11.9869 1.46055 11.6438 1.77003 11.382C2.0795 11.1203 2.456 10.9502 2.857 10.8911L9.974 9.85712C10.3228 9.80648 10.6541 9.67179 10.9392 9.46466C11.2244 9.25753 11.455 8.98419 11.611 8.66815L14.794 2.21912C14.9728 1.85398 15.2505 1.54635 15.5955 1.33118C15.9405 1.11601 16.3389 1.00195 16.7455 1.00195C17.1521 1.00195 17.5505 1.11601 17.8955 1.33118C18.2405 1.54635 18.5182 1.85398 18.697 2.21912V2.21912Z"
                  stroke="#92929C"
                  stroke-width="1.607"
                  stroke-miterlimit="10"
                />
              </svg>
            </i>

            <!-- pen icon  -->
            <i
              class="cursor-pointer block p-[8px] xl:p-[10px] rounded-full transition-colors ease-in-out duration-150 [@media(hover:hover)]:hover:bg-[#F1F1F5]"
            >
              <svg
                class="w-[24px] h-[24px] xl:w-[31px] xl:h-[31px]"
                width="31"
                height="31"
                viewBox="0 0 34 34"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M3.17671 22.8199L1.80971 27.9199L1.05171 30.7468C0.982774 31.0041 0.982762 31.2749 1.05168 31.5322C1.1206 31.7894 1.25601 32.0239 1.44432 32.2122C1.63263 32.4005 1.86718 32.536 2.12441 32.6049C2.38165 32.6738 2.65249 32.6738 2.90971 32.6049L5.73671 31.8469L11.1007 30.4099L31.8007 9.70984C32.1372 9.37242 32.3261 8.91536 32.3261 8.43885C32.3261 7.96234 32.1372 7.50527 31.8007 7.16785L26.4937 1.86084C26.3261 1.69388 26.1273 1.56157 25.9086 1.4715C25.6899 1.38143 25.4555 1.33539 25.219 1.33594C24.9824 1.3365 24.7483 1.3837 24.53 1.4748C24.3117 1.5659 24.1135 1.69914 23.9467 1.86689L3.17671 22.8199Z"
                  stroke="#92929C"
                  stroke-width="1.607"
                  stroke-miterlimit="10"
                />
                <path
                  d="M11.0813 30.4329L3.44434 22.7959"
                  stroke="#92929C"
                  stroke-width="1.607"
                  stroke-miterlimit="10"
                />
              </svg>
            </i>

            <!-- setting icon  -->
            <i
              class="cursor-pointer block p-[8px] xl:p-[10px] rounded-full transition-colors ease-in-out duration-150 [@media(hover:hover)]:hover:bg-[#F1F1F5]"
            >
              <svg
                class="w-[24px] h-[24px] xl:w-[31px] xl:h-[31px]"
                width="33"
                height="33"
                viewBox="0 0 33 33"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M16.1873 22.6478C19.3817 22.6478 21.9713 20.0582 21.9713 16.8638C21.9713 13.6694 19.3817 11.0798 16.1873 11.0798C12.9929 11.0798 10.4033 13.6694 10.4033 16.8638C10.4033 20.0582 12.9929 22.6478 16.1873 22.6478Z"
                  stroke="#92929C"
                  stroke-width="1.607"
                  stroke-miterlimit="10"
                />
                <path
                  d="M31.369 19.1819V14.5439C31.369 14.1991 31.232 13.8684 30.9882 13.6246C30.7444 13.3808 30.4138 13.2439 30.069 13.2439H28.065C27.8095 13.2434 27.5598 13.1671 27.3477 13.0247C27.1355 12.8823 26.9703 12.6802 26.873 12.4439L26.866 12.4279C26.7662 12.1913 26.7391 11.9304 26.7883 11.6783C26.8374 11.4263 26.9606 11.1946 27.142 11.0129L28.562 9.5929C28.8038 9.34937 28.9395 9.02008 28.9395 8.67688C28.9395 8.33368 28.8038 8.00445 28.562 7.76093L25.283 4.4809C25.0394 4.23877 24.7099 4.10284 24.3665 4.10284C24.0231 4.10284 23.6936 4.23877 23.45 4.4809L22.03 5.90088C21.8483 6.08229 21.6166 6.20548 21.3646 6.25464C21.1125 6.3038 20.8516 6.2767 20.615 6.17688L20.599 6.16992C20.3627 6.07262 20.1606 5.90743 20.0182 5.69525C19.8758 5.48308 19.7995 5.23343 19.799 4.97791V2.96991C19.799 2.62513 19.662 2.29446 19.4182 2.05066C19.1744 1.80686 18.8438 1.66992 18.499 1.66992H13.868C13.5232 1.66992 13.1926 1.80686 12.9488 2.05066C12.705 2.29446 12.568 2.62513 12.568 2.96991V4.97791C12.5675 5.23343 12.4912 5.48308 12.3488 5.69525C12.2064 5.90743 12.0043 6.07262 11.768 6.16992L11.752 6.17688C11.5154 6.2767 11.2545 6.3038 11.0024 6.25464C10.7504 6.20548 10.5187 6.08229 10.337 5.90088L8.917 4.4809C8.67343 4.23877 8.34394 4.10284 8.0005 4.10284C7.65706 4.10284 7.32757 4.23877 7.084 4.4809L3.804 7.76093C3.68354 7.88112 3.58797 8.02385 3.52276 8.18103C3.45755 8.33821 3.42399 8.50671 3.42399 8.67688C3.42399 8.84705 3.45755 9.01555 3.52276 9.17273C3.58797 9.32991 3.68354 9.4727 3.804 9.5929L5.224 11.0129C5.40524 11.1947 5.5282 11.4264 5.57718 11.6785C5.62616 11.9305 5.59894 12.1914 5.499 12.4279L5.493 12.4439C5.39569 12.6802 5.23051 12.8823 5.01834 13.0247C4.80616 13.1671 4.55653 13.2434 4.301 13.2439H2.3C1.95522 13.2439 1.62456 13.3808 1.38076 13.6246C1.13696 13.8684 1 14.1991 1 14.5439V19.1819C1 19.5267 1.13696 19.8573 1.38076 20.1011C1.62456 20.3449 1.95522 20.4819 2.3 20.4819H4.309C4.56453 20.4824 4.81416 20.5587 5.02634 20.7011C5.23851 20.8435 5.40369 21.0456 5.501 21.2819L5.507 21.2979C5.60694 21.5344 5.63416 21.7953 5.58518 22.0473C5.5362 22.2993 5.41324 22.531 5.232 22.7129L3.812 24.1329C3.56987 24.3764 3.43397 24.7059 3.43397 25.0494C3.43397 25.3928 3.56987 25.7223 3.812 25.9659L7.092 29.2459C7.33557 29.488 7.66506 29.6239 8.0085 29.6239C8.35194 29.6239 8.68143 29.488 8.925 29.2459L10.345 27.8259C10.5267 27.6445 10.7584 27.5213 11.0104 27.4722C11.2625 27.423 11.5234 27.4501 11.76 27.5499L11.776 27.5559C12.0124 27.6533 12.2147 27.8186 12.3571 28.031C12.4995 28.2434 12.5757 28.4932 12.576 28.7489V30.7569C12.576 31.1017 12.713 31.4324 12.9568 31.6761C13.2006 31.9199 13.5312 32.0569 13.876 32.0569H18.514C18.8588 32.0569 19.1894 31.9199 19.4332 31.6761C19.677 31.4324 19.814 31.1017 19.814 30.7569V28.7489C19.8143 28.4932 19.8905 28.2434 20.0329 28.031C20.1753 27.8186 20.3776 27.6533 20.614 27.5559L20.63 27.5499C20.8666 27.4501 21.1275 27.423 21.3796 27.4722C21.6316 27.5213 21.8633 27.6445 22.045 27.8259L23.465 29.2459C23.7086 29.488 24.0381 29.6239 24.3815 29.6239C24.7249 29.6239 25.0544 29.488 25.298 29.2459L28.577 25.9659C28.8191 25.7223 28.955 25.3928 28.955 25.0494C28.955 24.7059 28.8191 24.3764 28.577 24.1329L27.157 22.7129C26.9756 22.5312 26.8524 22.2995 26.8033 22.0475C26.7541 21.7955 26.7812 21.5345 26.881 21.2979L26.888 21.2819C26.9853 21.0456 27.1505 20.8435 27.3627 20.7011C27.5748 20.5587 27.8245 20.4824 28.08 20.4819H30.088C30.4295 20.4769 30.7553 20.3377 30.995 20.0945C31.2347 19.8512 31.369 19.5234 31.369 19.1819V19.1819Z"
                  stroke="#92929C"
                  stroke-width="1.607"
                  stroke-miterlimit="10"
                />
              </svg>
            </i>
          </div>
          <!-- user icon  -->
          <div class="flex w-full items-center justify-center">
            <span
              class="helvetica-font bg-[#F1F1F5] text-[35.17px] w-[40.33px] h-[40.33px] lg:w-[55.33px] lg:h-[55.33px] rounded-full p-1 text-[#92929C] flex items-center justify-center cursor-pointer"
            >
              <i
                ><svg
                  class="w-[26px] h-[26px] xl:w-[31px] xl:h-[31px]"
                  width="31"
                  height="31"
                  viewBox="0 0 23 29"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M11.4964 13.7871C14.8875 13.7871 17.6364 11.0381 17.6364 7.64708C17.6364 4.25605 14.8875 1.50708 11.4964 1.50708C8.10542 1.50708 5.35645 4.25605 5.35645 7.64708C5.35645 11.0381 8.10542 13.7871 11.4964 13.7871Z"
                    stroke="#92929C"
                    stroke-width="1.766"
                    stroke-miterlimit="10"
                  />
                  <path
                    d="M10.8842 17.2319H12.1062C14.5531 17.2319 16.8998 18.204 18.63 19.9342C20.3602 21.6644 21.3322 24.011 21.3322 26.4579V27.2249H1.6582V26.4579C1.6582 24.011 2.63023 21.6644 4.36044 19.9342C6.09065 18.204 8.43732 17.2319 10.8842 17.2319V17.2319Z"
                    stroke="#92929C"
                    stroke-width="1.766"
                    stroke-miterlimit="10"
                  />
                </svg>
              </i>
            </span>
          </div>
        </section>
      </div>

      <!-- **************nav side manue***********  -->
      <section
        :class="`hidden xl:block pt-28 ease-in-out duration-200  ${
          !sideNavCollapse
            ? 'transition-all   w-[65px]'
            : 'transition-all  w-[252px]'
        }  bg-[#F1F1F5] rounded-[42px_0_0_42px] ml-2 relative`"
      >
        <!-- nav no collpase icon  -->
        <i
          @click="sideNavCollapse = true"
          v-show="!sideNavCollapse"
          class="inline-block absolute top-12 -right-4 cursor-pointer z-[201]"
          ><svg
            width="32"
            height="32"
            viewBox="0 0 32 32"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <rect
              x="-0.25"
              y="0.25"
              width="31.5"
              height="31.5"
              rx="15.75"
              transform="matrix(-1 0 0 1 31.5 0)"
              fill="white"
              stroke="#D5D5DC"
              stroke-width="0.5"
            />
            <path
              d="M13.3599 23.3418L19.6798 16.6548C19.8856 16.4329 20 16.1415 20 15.8388C20 15.5362 19.8856 15.2447 19.6798 15.0228L13.3609 8.33783C13.2625 8.2313 13.1431 8.14629 13.0102 8.08815C12.8773 8.03001 12.7339 8 12.5889 8C12.4438 8 12.3004 8.03001 12.1675 8.08815C12.0347 8.14629 11.9153 8.2313 11.8169 8.33783C11.6108 8.55978 11.4962 8.85145 11.4962 9.15432C11.4962 9.4572 11.6108 9.74887 11.8169 9.97083L17.3639 15.8398L11.8169 21.7098C11.6108 21.9318 11.4962 22.2235 11.4962 22.5263C11.4962 22.8292 11.6108 23.1209 11.8169 23.3428C11.9153 23.4493 12.0346 23.5342 12.1674 23.5922C12.3002 23.6503 12.4436 23.6802 12.5886 23.6801C12.7335 23.68 12.8769 23.6499 13.0096 23.5917C13.1424 23.5335 13.2616 23.4484 13.3599 23.3418Z"
              fill="#696973"
            />
          </svg>
        </i>
        <!-- nav after collpase icon  -->
        <i
          @click="sideNavCollapse = false"
          v-show="sideNavCollapse"
          class="inline-block absolute top-12 -right-4 cursor-pointer z-[201]"
          ><svg
            width="32"
            height="32"
            viewBox="0 0 32 32"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <rect
              x="0.25"
              y="0.25"
              width="31.5"
              height="31.5"
              rx="15.75"
              fill="white"
              stroke="#D5D5DC"
              stroke-width="0.5"
            />
            <path
              d="M18.6401 23.3418L12.3202 16.6548C12.1144 16.4329 12 16.1415 12 15.8388C12 15.5362 12.1144 15.2447 12.3202 15.0228L18.6391 8.33783C18.7375 8.2313 18.8569 8.14629 18.9898 8.08815C19.1227 8.03001 19.2661 8 19.4111 8C19.5562 8 19.6996 8.03001 19.8325 8.08815C19.9653 8.14629 20.0847 8.2313 20.1831 8.33783C20.3892 8.55978 20.5038 8.85145 20.5038 9.15432C20.5038 9.4572 20.3892 9.74887 20.1831 9.97083L14.6361 15.8398L20.1831 21.7098C20.3892 21.9318 20.5038 22.2235 20.5038 22.5263C20.5038 22.8292 20.3892 23.1209 20.1831 23.3428C20.0847 23.4493 19.9654 23.5342 19.8326 23.5922C19.6998 23.6503 19.5564 23.6802 19.4114 23.6801C19.2665 23.68 19.1231 23.6499 18.9904 23.5917C18.8576 23.5335 18.7384 23.4484 18.6401 23.3418Z"
              fill="#696973"
            />
          </svg>
        </i>
        <!-- *******side manue main wrapper container  -->
        <main
          :class="`  ${
            !sideNavCollapse
              ? 'opacity-0 pointer-events-none'
              : ' transition-opacity ease-in-out delay-75 duration-200 opacity-100 pointer-events-auto'
          }`"
        >
          <!-- nav search bar and heading   -->
          <div class="px-6 space-y-14 mb-14">
            <h2
              class="popins-font font-bold text-[#1C1E21] text-xl lg:text-2xl"
            >
              My Courses
            </h2>
            <!-- search bar  -->
            <div class="bg-white border border-[#D5D5DC] flex gap-1 p-2">
              <input
                type="text"
                placeholder="search course name"
                class="roboto-font placeholder-[#92929C] text-[#92929C] text-[10px] w-full bg-transparent outline-none"
              />
              <!-- search icon  -->
              <i class="cursor-pointer"
                ><svg
                  width="15"
                  height="15"
                  viewBox="0 0 15 15"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M6.36248 11.848C9.38127 11.848 11.8285 9.41245 11.8285 6.40802C11.8285 3.40359 9.38127 0.968018 6.36248 0.968018C3.3437 0.968018 0.896484 3.40359 0.896484 6.40802C0.896484 9.41245 3.3437 11.848 6.36248 11.848Z"
                    stroke="#B5B5BD"
                    stroke-width="1.264"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M13.3916 13.401L10.2676 10.293"
                    stroke="#B5B5BD"
                    stroke-width="1.264"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                </svg>
              </i>
            </div>
          </div>
          <!-- ****************side links wrapper   -->
          <section class="space-y-8">
            <!-- manue #1  -->

            <div class="">
              <div
                @click="sideManueUpdates = !sideManueUpdates"
                class="px-6 flex w-full justify-between items-center select-none cursor-pointer"
              >
                <div class="gap-2 flex items-center">
                  <!-- manue icon  -->
                  <i>
                    <svg
                      width="27"
                      height="26"
                      viewBox="0 0 27 26"
                      fill="none"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path
                        d="M20.7961 1.00293H6.29613C5.59896 1.00161 4.92979 1.27717 4.43568 1.76902C3.94158 2.26087 3.66299 2.92878 3.66113 3.62595V20.674C3.66299 21.371 3.94162 22.0388 4.43575 22.5305C4.92988 23.0222 5.59905 23.2975 6.29613 23.2959H15.0081C15.3376 23.296 15.6552 23.1734 15.8991 22.9519L22.9991 16.4739C23.1336 16.3513 23.241 16.2019 23.3145 16.0354C23.388 15.8689 23.426 15.6889 23.4261 15.5069V3.62195C23.4232 2.92634 23.1449 2.2602 22.6519 1.76935C22.159 1.27851 21.4918 1.00293 20.7961 1.00293V1.00293Z"
                        stroke="#92929C"
                        stroke-width="0.935"
                        stroke-miterlimit="10"
                      />
                      <path
                        d="M15.5254 23.2918V18.7029C15.5262 18.3575 15.595 18.0157 15.7279 17.697C15.8608 17.3783 16.0552 17.0889 16.3 16.8453C16.5448 16.6017 16.8352 16.4087 17.1546 16.2774C17.4739 16.1461 17.8161 16.0789 18.1614 16.0798H23.1034"
                        stroke="#92929C"
                        stroke-width="0.935"
                        stroke-miterlimit="10"
                      />
                      <path
                        d="M6.95898 5.58887H17.502"
                        stroke="#92929C"
                        stroke-width="0.935"
                        stroke-miterlimit="10"
                      />
                      <path
                        d="M6.95898 19.3579H12.23"
                        stroke="#92929C"
                        stroke-width="0.935"
                        stroke-miterlimit="10"
                      />
                      <path
                        d="M6.95898 14.7681H14.866"
                        stroke="#92929C"
                        stroke-width="0.935"
                        stroke-miterlimit="10"
                      />
                      <path
                        d="M6.95898 10.179H20.137"
                        stroke="#92929C"
                        stroke-width="0.935"
                        stroke-miterlimit="10"
                      />
                    </svg>
                  </i>
                  <span
                    class="roboto-font font-bold text-[#1C1E21] text-xs md:text-sm"
                    >Updates</span
                  >
                </div>
                <!-- chev right icon  -->
                <i v-show="!sideManueUpdates" class="cursor-pointer">
                  <svg
                    width="7"
                    height="11"
                    viewBox="0 0 7 11"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M1.98898 10.273L5.98898 6.01898C6.11913 5.87728 6.19135 5.69188 6.19134 5.49948C6.19134 5.30708 6.11913 5.12169 5.98898 4.97998L1.98898 0.72699C1.92687 0.659146 1.85131 0.604965 1.76712 0.567902C1.68293 0.530838 1.59195 0.511719 1.49997 0.511719C1.40799 0.511719 1.317 0.530838 1.23282 0.567902C1.14863 0.604965 1.07307 0.659146 1.01096 0.72699C0.880809 0.868694 0.808593 1.05409 0.808593 1.24649C0.808593 1.43889 0.880809 1.62429 1.01096 1.76599L4.52298 5.49899L1.01096 9.23398C0.880809 9.37568 0.808594 9.56108 0.808594 9.75348C0.808594 9.94588 0.880809 10.1313 1.01096 10.273C1.07307 10.3408 1.14863 10.395 1.23282 10.4321C1.317 10.4691 1.40799 10.4883 1.49997 10.4883C1.59195 10.4883 1.68293 10.4691 1.76712 10.4321C1.85131 10.395 1.92687 10.3408 1.98898 10.273Z"
                      fill="#92929C"
                    />
                  </svg>
                </i>
                <!-- when no collapse  -->
                <i v-show="sideManueUpdates" class="cursor-pointer">
                  <svg
                    width="11"
                    height="7"
                    viewBox="0 0 11 7"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M0.72702 1.98898L4.98102 5.98898C5.12272 6.11913 5.30812 6.19135 5.50052 6.19135C5.69292 6.19135 5.87831 6.11913 6.02002 5.98898L10.273 1.98898C10.3409 1.92687 10.395 1.85131 10.4321 1.76712C10.4692 1.68293 10.4883 1.59195 10.4883 1.49997C10.4883 1.40799 10.4692 1.317 10.4321 1.23282C10.395 1.14863 10.3409 1.07307 10.273 1.01096C10.1313 0.880809 9.94591 0.808594 9.75351 0.808594C9.56111 0.808594 9.37571 0.880809 9.23401 1.01096L5.50101 4.52298L1.76602 1.01096C1.62432 0.880809 1.43892 0.808594 1.24652 0.808594C1.05412 0.808594 0.868725 0.880809 0.72702 1.01096C0.659177 1.07307 0.604996 1.14863 0.567932 1.23282C0.530869 1.317 0.511719 1.40799 0.511719 1.49997C0.511719 1.59195 0.530869 1.68293 0.567932 1.76712C0.604996 1.85131 0.659177 1.92687 0.72702 1.98898Z"
                      fill="#92929C"
                    />
                  </svg>
                </i>
              </div>
              <!-- ***********sub manues  -->
              <!-- sub manue wrapper  -->
              <section v-show="sideManueUpdates">
                <!-- sub manue link #1 wrapper -->
                <div class="">
                  <div
                    @click="sideSubManueUpdates = !sideSubManueUpdates"
                    class="pl-8 flex gap-2 pt-10 pb-3 items-center cursor-pointer"
                  >
                    <!-- sub manue header icon  -->
                    <i v-show="!sideSubManueUpdates"
                      ><svg
                        width="24"
                        height="24"
                        viewBox="0 0 24 24"
                        fill="none"
                        xmlns="http://www.w3.org/2000/svg"
                      >
                        <path
                          d="M12.0002 19.885C16.3765 19.885 19.9242 16.3548 19.9242 12C19.9242 7.64523 16.3765 4.11499 12.0002 4.11499C7.62387 4.11499 4.07617 7.64523 4.07617 12C4.07617 16.3548 7.62387 19.885 12.0002 19.885Z"
                          stroke="#171724"
                          stroke-width="0.952"
                          stroke-linejoin="round"
                        />
                        <path
                          d="M16.1937 12H7.80371"
                          stroke="#171724"
                          stroke-width="0.952"
                          stroke-linejoin="round"
                        />
                        <path
                          d="M11.999 16.1949L11.999 7.80493"
                          stroke="#171724"
                          stroke-width="0.952"
                          stroke-linejoin="round"
                        />
                      </svg>
                    </i>
                    <!-- when collapse  -->
                    <i v-show="sideSubManueUpdates"
                      ><svg
                        width="24"
                        height="24"
                        viewBox="0 0 24 24"
                        fill="none"
                        xmlns="http://www.w3.org/2000/svg"
                      >
                        <path
                          d="M12.0002 19.885C16.3765 19.885 19.9242 16.3548 19.9242 12C19.9242 7.64523 16.3765 4.11499 12.0002 4.11499C7.62387 4.11499 4.07617 7.64523 4.07617 12C4.07617 16.3548 7.62387 19.885 12.0002 19.885Z"
                          stroke="#171724"
                          stroke-width="0.952"
                          stroke-linejoin="round"
                        />
                        <path
                          d="M16.1937 12H7.80371"
                          stroke="#171724"
                          stroke-width="0.952"
                          stroke-linejoin="round"
                        />
                      </svg>
                    </i>
                    <!-- sub manue header text  -->
                    <span
                      class="roboto-font font-light text-[12px] text-[#171724]"
                      >Workshop Warm-up Sessions</span
                    >
                  </div>
                  <!-- ****sub manue linkss  -->
                  <!-- wrapper  -->
                  <div v-if="sideSubManueUpdates">
                    <div
                      class="pl-16 py-4 [@media(hover:hover)]:hover:bg-[#D5D5DC] transition-colors ease-in-out duration-200 cursor-pointer select-none"
                    >
                      <span
                        class="roboto-font font-light text-[11px] text-[#1C1E21]"
                        >Load Your Profile Picture</span
                      >
                    </div>
                    <div
                      class="pl-16 py-4 [@media(hover:hover)]:hover:bg-[#D5D5DC] transition-colors ease-in-out duration-200 cursor-pointer select-none"
                    >
                      <span
                        class="roboto-font font-light text-[11px] text-[#1C1E21]"
                        >Load Your Profile Picture</span
                      >
                    </div>
                    <div
                      class="pl-16 py-4 [@media(hover:hover)]:hover:bg-[#D5D5DC] transition-colors ease-in-out duration-200 cursor-pointer select-none"
                    >
                      <span
                        class="roboto-font font-light text-[11px] text-[#1C1E21]"
                        >Load Your Profile Picture</span
                      >
                    </div>
                    <div
                      class="pl-16 py-4 [@media(hover:hover)]:hover:bg-[#D5D5DC] transition-colors ease-in-out duration-200 cursor-pointer select-none"
                    >
                      <span
                        class="roboto-font font-light text-[11px] text-[#1C1E21]"
                        >Load Your Profile Picture</span
                      >
                    </div>
                  </div>
                </div>
              </section>
            </div>
            <!-- manue item #2  -->
            <div class="">
              <div
                @click="sideManueCourses = !sideManueCourses"
                class="px-6 flex w-full justify-between items-center select-none cursor-pointer"
              >
                <div class="gap-2 flex items-center">
                  <!-- manue icon  -->
                  <i>
                    <svg
                      width="27"
                      height="25"
                      viewBox="0 0 27 25"
                      fill="none"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path
                        d="M21.5118 22.8281C22.0638 23.4486 22.8192 23.8516 23.642 23.9647C24.4647 24.0778 25.3008 23.8936 25.9998 23.4451C25.4588 23.1398 24.9931 22.7173 24.6366 22.2086C24.2802 21.6999 24.0421 21.1178 23.9398 20.5051C24.8177 19.209 25.2854 17.6786 25.2818 16.1131C25.2871 14.3621 24.7111 12.6589 23.6441 11.2705C22.5772 9.8821 21.0796 8.88707 19.3862 8.44149C17.6928 7.9959 15.8995 8.12495 14.2873 8.80837C12.6752 9.49179 11.3355 10.691 10.4783 12.2178C9.62105 13.7446 9.29483 15.5128 9.55076 17.245C9.80669 18.9772 10.6303 20.5755 11.8924 21.7892C13.1545 23.0029 14.7838 23.7634 16.5247 23.9514C18.2656 24.1395 20.0196 23.7444 21.5118 22.8281V22.8281Z"
                        stroke="#92929C"
                        stroke-width="0.935"
                        stroke-miterlimit="10"
                      />
                      <path
                        d="M7.50495 15.1871C6.85479 15.0075 6.23281 14.7383 5.65695 14.3871C5.15047 14.9549 4.45826 15.3236 3.70451 15.4271C2.95075 15.5307 2.18476 15.3623 1.54395 14.9521C2.04015 14.6729 2.46738 14.2859 2.79414 13.8197C3.12089 13.3534 3.33885 12.8198 3.43195 12.2581C2.62785 11.0694 2.19998 9.66623 2.20395 8.23109C2.21284 6.47902 2.85461 4.78917 4.01103 3.47291C5.16745 2.15665 6.7606 1.30264 8.49695 1.06825C10.2333 0.833854 11.9959 1.23488 13.4599 2.1974C14.9239 3.15992 15.9908 4.6191 16.464 6.3061"
                        stroke="#92929C"
                        stroke-width="0.935"
                        stroke-miterlimit="10"
                      />
                    </svg>
                  </i>
                  <span
                    class="roboto-font font-bold text-[#1C1E21] text-xs md:text-sm"
                    >Courses</span
                  >
                </div>
                <!-- chev right icon  -->
                <i v-show="!sideManueCourses" class="cursor-pointer">
                  <svg
                    width="7"
                    height="11"
                    viewBox="0 0 7 11"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M1.98898 10.273L5.98898 6.01898C6.11913 5.87728 6.19135 5.69188 6.19134 5.49948C6.19134 5.30708 6.11913 5.12169 5.98898 4.97998L1.98898 0.72699C1.92687 0.659146 1.85131 0.604965 1.76712 0.567902C1.68293 0.530838 1.59195 0.511719 1.49997 0.511719C1.40799 0.511719 1.317 0.530838 1.23282 0.567902C1.14863 0.604965 1.07307 0.659146 1.01096 0.72699C0.880809 0.868694 0.808593 1.05409 0.808593 1.24649C0.808593 1.43889 0.880809 1.62429 1.01096 1.76599L4.52298 5.49899L1.01096 9.23398C0.880809 9.37568 0.808594 9.56108 0.808594 9.75348C0.808594 9.94588 0.880809 10.1313 1.01096 10.273C1.07307 10.3408 1.14863 10.395 1.23282 10.4321C1.317 10.4691 1.40799 10.4883 1.49997 10.4883C1.59195 10.4883 1.68293 10.4691 1.76712 10.4321C1.85131 10.395 1.92687 10.3408 1.98898 10.273Z"
                      fill="#92929C"
                    />
                  </svg>
                </i>
                <!-- when no collapse  -->
                <i v-show="sideManueCourses" class="cursor-pointer">
                  <svg
                    width="11"
                    height="7"
                    viewBox="0 0 11 7"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M0.72702 1.98898L4.98102 5.98898C5.12272 6.11913 5.30812 6.19135 5.50052 6.19135C5.69292 6.19135 5.87831 6.11913 6.02002 5.98898L10.273 1.98898C10.3409 1.92687 10.395 1.85131 10.4321 1.76712C10.4692 1.68293 10.4883 1.59195 10.4883 1.49997C10.4883 1.40799 10.4692 1.317 10.4321 1.23282C10.395 1.14863 10.3409 1.07307 10.273 1.01096C10.1313 0.880809 9.94591 0.808594 9.75351 0.808594C9.56111 0.808594 9.37571 0.880809 9.23401 1.01096L5.50101 4.52298L1.76602 1.01096C1.62432 0.880809 1.43892 0.808594 1.24652 0.808594C1.05412 0.808594 0.868725 0.880809 0.72702 1.01096C0.659177 1.07307 0.604996 1.14863 0.567932 1.23282C0.530869 1.317 0.511719 1.40799 0.511719 1.49997C0.511719 1.59195 0.530869 1.68293 0.567932 1.76712C0.604996 1.85131 0.659177 1.92687 0.72702 1.98898Z"
                      fill="#92929C"
                    />
                  </svg>
                </i>
              </div>
              <!-- ***********sub manues  -->
              <!-- sub manue wrapper  -->
              <section v-show="sideManueCourses">
                <!-- sub manue link #1 wrapper -->
                <div class="">
                  <div
                    @click="sideSubManueWorkshop = !sideSubManueWorkshop"
                    class="pl-8 flex gap-2 pt-10 pb-3 items-center cursor-pointer"
                  >
                    <!-- sub manue header icon  -->
                    <i v-show="!sideSubManueWorkshop"
                      ><svg
                        width="24"
                        height="24"
                        viewBox="0 0 24 24"
                        fill="none"
                        xmlns="http://www.w3.org/2000/svg"
                      >
                        <path
                          d="M12.0002 19.885C16.3765 19.885 19.9242 16.3548 19.9242 12C19.9242 7.64523 16.3765 4.11499 12.0002 4.11499C7.62387 4.11499 4.07617 7.64523 4.07617 12C4.07617 16.3548 7.62387 19.885 12.0002 19.885Z"
                          stroke="#171724"
                          stroke-width="0.952"
                          stroke-linejoin="round"
                        />
                        <path
                          d="M16.1937 12H7.80371"
                          stroke="#171724"
                          stroke-width="0.952"
                          stroke-linejoin="round"
                        />
                        <path
                          d="M11.999 16.1949L11.999 7.80493"
                          stroke="#171724"
                          stroke-width="0.952"
                          stroke-linejoin="round"
                        />
                      </svg>
                    </i>
                    <!-- when collapse  -->
                    <i v-show="sideSubManueWorkshop"
                      ><svg
                        width="24"
                        height="24"
                        viewBox="0 0 24 24"
                        fill="none"
                        xmlns="http://www.w3.org/2000/svg"
                      >
                        <path
                          d="M12.0002 19.885C16.3765 19.885 19.9242 16.3548 19.9242 12C19.9242 7.64523 16.3765 4.11499 12.0002 4.11499C7.62387 4.11499 4.07617 7.64523 4.07617 12C4.07617 16.3548 7.62387 19.885 12.0002 19.885Z"
                          stroke="#171724"
                          stroke-width="0.952"
                          stroke-linejoin="round"
                        />
                        <path
                          d="M16.1937 12H7.80371"
                          stroke="#171724"
                          stroke-width="0.952"
                          stroke-linejoin="round"
                        />
                      </svg>
                    </i>
                    <!-- sub manue header text  -->
                    <span
                      class="roboto-font font-light text-[12px] text-[#171724]"
                      >Workshop Warm-up Sessions</span
                    >
                  </div>
                  <!-- ****sub manue linkss  -->
                  <!-- wrapper  -->
                  <div v-if="sideSubManueWorkshop">
                    <div
                      class="pl-16 py-4 [@media(hover:hover)]:hover:bg-[#D5D5DC] transition-colors ease-in-out duration-200 cursor-pointer select-none"
                    >
                      <span
                        class="roboto-font font-light text-[11px] text-[#1C1E21]"
                        >Load Your Profile Picture</span
                      >
                    </div>
                    <div
                      class="pl-16 py-4 [@media(hover:hover)]:hover:bg-[#D5D5DC] transition-colors ease-in-out duration-200 cursor-pointer select-none"
                    >
                      <span
                        class="roboto-font font-light text-[11px] text-[#1C1E21]"
                        >Load Your Profile Picture</span
                      >
                    </div>
                    <div
                      class="pl-16 py-4 [@media(hover:hover)]:hover:bg-[#D5D5DC] transition-colors ease-in-out duration-200 cursor-pointer select-none"
                    >
                      <span
                        class="roboto-font font-light text-[11px] text-[#1C1E21]"
                        >Load Your Profile Picture</span
                      >
                    </div>
                    <div
                      class="pl-16 py-4 [@media(hover:hover)]:hover:bg-[#D5D5DC] transition-colors ease-in-out duration-200 cursor-pointer select-none"
                    >
                      <span
                        class="roboto-font font-light text-[11px] text-[#1C1E21]"
                        >Load Your Profile Picture</span
                      >
                    </div>
                  </div>
                </div>
              </section>
            </div>
          </section>
        </main>
      </section>
    </nav>
  </div>
</template>

<script>
export default {
  name: "NavbarVue",
  props: ["navSelected"],
  data() {
    return {
      sideNavCollapse: false,
      sideManueCourses: false,
      sideSubManueWorkshop: false,
      sideManueUpdates: false,
      sideSubManueUpdates: false,
      homeIconSelected: false,
      paperIconSelected: false,
      mobileBurgerManue: false,
    }
  },
}
</script>

<style></style>
