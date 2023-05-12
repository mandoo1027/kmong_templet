<template>
  <div class="login-page mx-auto lg:pt-[203px] pt-14 lg:w-[974px] w-5/6">
        <figure class="logo mx-auto lg:w-[503px] w-1/2 lg-mb-[175px] mb-16">
          <img src="/assets/images/common/logo.svg" alt="BIZDRM" />
        </figure>
        <form action="" class="">
          <fieldset class="w-full">
            <legend class="blind">로그인</legend>
            <div class="input-wrap w-full">
              <input
                class="w-full rounded-sm border-solid border-black text-md px-2.5 py-2.5 border-2 lg:text-4xl lg:border-4 lg:px-[57px] lg:py-8"
                type="text"
                placeholder="아이디"
                required
              />
            </div>
            <div class="input-wrap w-full lg:mt-12 mt-3">
              <input
                class="w-full rounded-sm border-solid border-black text-md px-2.5 py-2.5 border-2 lg:text-4xl lg:border-4 lg:px-[57px] lg:py-8"
                type="password"
                placeholder="비밀번호"
                required
              />
            </div>
          </fieldset>
          <div class="util-wrap">
            <div class="checkbox-wrap flex items-center justify-end lg:mt-20 mt-3">
              <input class="hidden" type="checkbox" name="" id="remember" />
              <label class="lg:text-[40px] text-md flex items-center" for="remember"
                ><span class="check-img lg:w-[67px] lg:h-[51px] lg:mr-[31px] w-8 h-6 mr-3 bg-white border-1 border-black"></span>기억하기</label
              >
            </div>
            <a href="" class="lg:mt-8 lg:text-4xl mt-4 text-md text-black no-underline">아이디/비밀번호 찾기</a>
          </div>
          <div class="button-wrap lg:mt-8 mt-2.5">
            <button class="lg:text-4xl text-md w-full lg:py-8 py-3.5 text-white leading-none bg-biz-red">로그인</button>
            <a
             href="/login/signup"
              class="inline-block lg:text-4xl lg:mt-6 lg:py-8 text-md mt-2 w-full py-3.5 text-white text-center no-underline leading-none bg-biz-gray"
              >회원가입</a
            >
          </div>
        </form>
      </div>
</template>