
<template>
  <main>
     <div class="main-page w-full mx-auto xl:w-[1440px]">
        <section class="main-vis h-fit xl:h-[698px]">
          <div class="flex items-center h-full py-[100px]">
            <h2 class="text-xl text-white font-bold pl-[20px] lg:text-4xl lg:pl-[120px]">BIZDRM으로,<br />마케팅 자동화도 SMART하게</h2>
          </div>
        </section>
        <section class="main-service py-[50px] lg:pt-[65px] lg:pb-[93px]">
          <h2 class="text-xl font-bold mb-12 text-center lg:pl-12">서비스 소개</h2>
          <!-- PC -->
          <ul class="hidden justify-between mx-auto xl:flex xl:w-[1082px]">
            <li class="text-center">
              <figure class="grid place-content-center shrink-0 bg-[#faeef1] rounded-xl mx-auto w-[126px] h-[126px]">
                <img src="/assets/images/main/icon_main_01.svg" alt="" />
              </figure>
              <figcaption class="my-12 font-bold text-2xl">문자/메세지 발송</figcaption>
              <p class="text-lg text-center">
                문자/메세지를 그룹별로, 원하는대로<br />
                발송하여 강력한 타겟마케팅<br />
                효과
              </p>
            </li>
            <li class="text-center">
              <figure class="grid place-content-center shrink-0 bg-[#faeef1] rounded-xl mx-auto w-[126px] h-[126px]">
                <img src="/assets/images/main/icon_main_02.svg" alt="" />
              </figure>
              <figcaption class="my-12 font-bold text-2xl">편리함</figcaption>
              <p class="text-lg text-center">
                쉬운 인터페이스로 어려움 없이<br />
                단 몇번의 클릭으로 진행하는<br />
                마케팅 활동
              </p>
            </li>
            <li class="text-center">
              <figure class="grid place-content-center shrink-0 bg-[#faeef1] rounded-xl mx-auto w-[126px] h-[126px]">
                <img src="/assets/images/main/icon_main_03.svg" alt="" />
              </figure>
              <figcaption class="my-12 font-bold text-2xl">맞춤형 마케팅</figcaption>
              <p class="text-lg text-center">
                대시보드를 통한 DB분석으로<br />
                더욱 고도화된 맞춤형 마케팅 <br />
                설계 가능
              </p>
            </li>
          </ul>
          <!-- MOBILE  -->
          <div class="swiper mainSwiper w-[90%] xl:hidden pb-5">
            <ul class="swiper-wrapper">
              <li class="swiper-slide bg-white py-2 w-[80%] text-center">
                <figure class="grid place-content-center p-4 shrink-0 bg-[#faeef1] rounded-xl mx-auto w-[100px] h-[100px]">
                  <img src="/assets/images/main/icon_main_01.svg" alt="" />
                </figure>
                <figcaption class="my-12 font-bold text-2xl">문자/메세지 발송</figcaption>
                <p class="text-lg text-center">
                  문자/메세지를 그룹별로, 원하는대로<br />
                  발송하여 강력한 타겟마케팅<br />
                  효과
                </p>
              </li>
              <li class="swiper-slide bg-white py-2 w-[80%] text-center">
                <figure class="grid place-content-center p-4 shrink-0 bg-[#faeef1] rounded-xl mx-auto w-[100px] h-[100px]">
                  <img src="/assets/images/main/icon_main_02.svg" alt="" />
                </figure>
                <figcaption class="my-12 font-bold text-2xl">편리함</figcaption>
                <p class="text-lg text-center">
                  쉬운 인터페이스로 어려움 없이<br />
                  단 몇번의 클릭으로 진행하는<br />
                  마케팅 활동
                </p>
              </li>
              <li class="swiper-slide bg-white py-2 w-[80%] text-center">
                <figure class="grid place-content-center p-4 shrink-0 bg-[#faeef1] rounded-xl mx-auto w-[100px] h-[100px]">
                  <img src="/assets/images/main/icon_main_03.svg" alt="" />
                </figure>
                <figcaption class="my-12 font-bold text-2xl">맞춤형 마케팅</figcaption>
                <p class="text-lg text-center">
                  대시보드를 통한 DB분석으로<br />
                  더욱 고도화된 맞춤형 마케팅 <br />
                  설계 가능
                </p>
              </li>
            </ul>
            <div class="swiper-pagination"></div>
          </div>
        </section>
        <section class="main-recommend">
          <figure class="h-fit">
            <img class="hidden lg:block" src="/assets/images/main/main_recommend.jpg" alt="" />
            <img class="block lg:hidden" src="/assets/images/main/main_recommend_mob.jpg" alt="" />
          </figure>
        </section>
        <section class="main-msg">
          <figure class="h-fit">
            <img class="hidden lg:block" src="/assets/images/main/main_msg.jpg" alt="" />
            <img class="block lg:hidden" src="/assets/images/main/main_msg_mob.jpg" alt="" />
          </figure>
        </section>
      </div>
  </main>
</template>
