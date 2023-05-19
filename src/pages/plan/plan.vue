<!-- <script>
const swiper = new Swiper(".planSwiper", {
  effect: "coverflow",
  grabCursor: true,
  centeredSlides: true,
  slidesPerView: "auto",
  coverflowEffect: {
    rotate: 50,
    stretch: 0,
    depth: 100,
    modifier: 1,
    slideShadows: true,
  },
  pagination: {
    el: ".swiper-pagination",
  },
});
</script> -->
<template>
  <div class="plan-page">
    <section
      class="plan-vis h-fit px-[25px] py-[50px] lg:h-[247px] lg:pt-[86px] lg:pb-[97px]"
    >
      <hgroup class="text-center">
        <h2 class="text-xl text-white font-bold lg:text-2xl">플랜 및 가격</h2>
        <p class="text-white mt-3 text-base">
          나의 상황에 맞는 알맞는 최적의 플랜을 찾아 보세요!
        </p>
      </hgroup>
    </section>
    <section class="plan-list py-[80px] lg:py-[166px]">
      <!-- PC -->
      <ul class="hidden justify-center gap-[20px] lg:gap-[60px] lg:flex">
        <li
          class="plan-card flex-col flex justify-between items-center relative bg-white w-[80%] h-[350px] px-[10px] pt-[18px] pb-[27px] lg:w-[367px] lg:h-[556px] lg:px-[10px] lg:pt-[38px] lg:pb-[47px]"
        >
          <h3 class="text-2xl text-center"><b>BASIC</b></h3>
          <p class="text-2xl text-center leading-relaxed text-center">
            리드수 1,000명<br />
            광고노출/300회
          </p>
          <div class="text-center">
            <p class="text-biz-red text-2xl text-center">월 <b>100,000원</b></p>
            <button
              class="relative font-bold py-3 text-white text-center text-sm leading-none bg-biz-red"
            >
              선택하기
            </button>
          </div>
        </li>
        <li
          class="plan-card best-selling pro-plan-card flex-col flex justify-between items-center relative bg-white w-[80%] h-[350px] px-[10px] pt-[18px] pb-[27px] lg:w-[367px] lg:h-[556px] lg:px-[10px] lg:pt-[38px] lg:pb-[47px]"
        >
          <h3 class="text-2xl text-center"><b>PRO+</b></h3>
          <p class="text-2xl text-center leading-relaxed text-center">
            리드수 2,500명<br />
            광고노출/500회
          </p>
          <div class="text-center">
            <p class="text-biz-red text-2xl text-center">월 <b>300,000원</b></p>
            <button
              class="relative font-bold py-3 text-white text-center text-sm leading-none bg-biz-red"
            >
              선택하기
            </button>
          </div>
        </li>
        <li
          class="plan-card special-plan-card flex-col flex justify-between items-center relative bg-white w-[80%] h-[350px] px-[10px] pt-[18px] pb-[27px] lg:w-[367px] lg:h-[556px] lg:px-[10px] lg:pt-[38px] lg:pb-[47px]"
        >
          <h3 class="text-2xl text-center"><b>SPECIAL++</b></h3>
          <p class="text-2xl text-center leading-relaxed text-center">
            리드수 10,000명<br />
            광고노출/3,000회<br />
            전담인력 배정
          </p>
          <div class="text-center">
            <p class="text-biz-red text-2xl text-center">월 <b>500,000원</b></p>
            <button
              class="relative font-bold py-3 text-white text-center text-sm leading-none bg-biz-red"
            >
              선택하기
            </button>
          </div>
        </li>
      </ul>
      <!-- MOBILE  -->

      <swiper
        :effect="'coverflow'"
        :grabCursor="true"
        :centeredSlides="true"
        :slidesPerView="'auto'"
        :coverflowEffect="{
          rotate: 50,
          stretch: 0,
          depth: 100,
          slideShadows: true,
        }"
        :pagination="true"
        :modules="modules"
        class="mySwiper h-[400px] lg:hidden pt-3 pb-10 sm:h-[700px] mobile-only"
      >
        <swiper-slide
          ><div
            class="plan-card flex-col flex justify-between items-center relative bg-white h-full px-[10px] pt-[18px] pb-[27px]"
          >
            <h3 class="text-xl text-center"><b>BASIC</b></h3>
            <p class="text-xl text-center leading-relaxed text-center">
              리드수 1,000명<br />
              광고노출/300회
            </p>
            <div class="text-center">
              <p class="text-biz-red text-xl text-center">
                월 <b>100,000원</b>
              </p>
              <button
                class="relative font-bold py-3 text-white text-center text-sm leading-none bg-biz-red"
              >
                선택하기
              </button>
            </div>
          </div> </swiper-slide
        ><swiper-slide
          ><div
            class="plan-card best-selling pro-plan-card flex-col flex justify-between items-center relative bg-white h-full px-[10px] py-[27px]"
          >
            <h3 class="text-xl text-center"><b>PRO+</b></h3>
            <p class="text-xl text-center leading-relaxed text-center">
              리드수 2,500명<br />
              광고노출/500회
            </p>
            <div class="text-center">
              <p class="text-biz-red text-xl text-center">
                월 <b>300,000원</b>
              </p>
              <button
                class="relative font-bold py-3 text-white text-center text-sm leading-none bg-biz-red"
              >
                선택하기
              </button>
            </div>
          </div></swiper-slide
        ><swiper-slide
          ><div
            class="plan-card special-plan-card flex-col flex justify-between items-center relative bg-white h-full px-[10px] py-[27px]"
          >
            <h3 class="text-xl text-center"><b>SPECIAL++</b></h3>
            <p class="text-xl text-center leading-relaxed text-center">
              리드수 10,000명<br />
              광고노출/3,000회<br />
              전담인력 배정
            </p>
            <div class="text-center">
              <p class="text-biz-red text-xl text-center">
                월 <b>500,000원</b>
              </p>
              <button
                class="relative font-bold py-3 text-white text-center text-sm leading-none bg-biz-red"
              >
                선택하기
              </button>
            </div>
          </div></swiper-slide
        >
      </swiper>

      <!-- <div
        class="swiper planSwiper h-[400px] lg:hidden pt-3 pb-10 sm:h-[700px]"
      >
        <ul class="swiper-wrapper">
          <li
            class="swiper-slide plan-card flex-col flex justify-between items-center relative bg-white w-[80%] h-full px-[10px] pt-[18px] pb-[27px]"
          >
            <h3 class="text-xl text-center"><b>BASIC</b></h3>
            <p class="text-xl text-center leading-relaxed text-center">
              리드수 1,000명<br />
              광고노출/300회
            </p>
            <div class="text-center">
              <p class="text-biz-red text-xl text-center">
                월 <b>100,000원</b>
              </p>
              <button
                class="relative font-bold py-3 text-white text-center text-sm leading-none bg-biz-red"
              >
                선택하기
              </button>
            </div>
          </li>
          <li
            class="swiper-slide plan-card best-selling pro-plan-card flex-col flex justify-between items-center relative bg-white w-[80%] h-full px-[10px] py-[27px]"
          >
            <h3 class="text-xl text-center"><b>PRO+</b></h3>
            <p class="text-xl text-center leading-relaxed text-center">
              리드수 2,500명<br />
              광고노출/500회
            </p>
            <div class="text-center">
              <p class="text-biz-red text-xl text-center">
                월 <b>300,000원</b>
              </p>
              <button
                class="relative font-bold py-3 text-white text-center text-sm leading-none bg-biz-red"
              >
                선택하기
              </button>
            </div>
          </li>
          <li
            class="swiper-slide plan-card special-plan-card flex-col flex justify-between items-center relative bg-white w-[80%] h-full px-[10px] py-[27px]"
          >
            <h3 class="text-xl text-center"><b>SPECIAL++</b></h3>
            <p class="text-xl text-center leading-relaxed text-center">
              리드수 10,000명<br />
              광고노출/3,000회<br />
              전담인력 배정
            </p>
            <div class="text-center">
              <p class="text-biz-red text-xl text-center">
                월 <b>500,000원</b>
              </p>
              <button
                class="relative font-bold py-3 text-white text-center text-sm leading-none bg-biz-red"
              >
                선택하기
              </button>
            </div>
          </li>
        </ul>
        <div class="swiper-pagination"></div>
      </div> -->
    </section>
  </div>
</template>

<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css";

import "swiper/css/effect-coverflow";
import "swiper/css/pagination";

// import required modules
import { EffectCoverflow, Pagination } from "swiper";

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [EffectCoverflow, Pagination],
    };
  },
};
</script>

<style>
.mySwiper .swiper-slide {
  max-width: 80%;
  max-height: 80%;

  transform: scale(0.8);
  opacity: 0.8;
}

.mySwiper .swiper-slide.swiper-slide-active,
.mySwiper .swiper-slide.swiper-slide-next {
  transform: scale(1);
  opacity: 1;
}

.mobile-only {
  display: none;
}

.desktop-only {
  display: block;
}

@media (max-width: 1023px) {
  /* 모바일 화면 크기로 조정 */
  .mobile-only {
    display: block; /* 모바일 화면에서 표시 */
  }
}
</style>
