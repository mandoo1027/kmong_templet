<template>
 <div class="signup-page bg-gray-f5">
        <div class="w-[90%] lg:w-[384px] mx-auto pt-[60px] pb-[100px]">
          <figure class="logo">
            <img src="/assets/images/common/logo.svg" alt="BIZDRM" />
          </figure>
          <form action="">
            <fieldset>
              <legend class="text-center font-bold mb-10">비즈디알엠 회원가입</legend>
              <ul>
                <li class="mb-8">
                  <div class="signup-check-box">
                    <input type="checkbox" name="" id="checkAll" />
                    <label class="flex items-center" for="checkAll">
                      <span class="check-img"></span>
                      <span class="underline font-bold text-sm"
                        >비즈디알엠 이용약관, 개인정보 수집 및 이용, 프로모션 정보<br class="hidden lg:block" />
                        수신(선택)에 모두 동의합니다.</span
                      ></label
                    >
                  </div>
                </li>
                <li class="mb-8">
                  <div class="signup-check-box mb-3">
                    <input type="checkbox" name="" id="agreeTerms" required />
                    <label class="flex items-center" for="agreeTerms">
                      <span class="check-img"></span>
                      <span class="underline font-bold text-sm">비즈디알엠 이용 약관 동의</span
                      ><small class="text-sm text-biz-red ml-px">(필수)</small></label
                    >
                  </div>
                  <div class="signup-content-box text-xs">
                    제1조(목적) 이 약관은 주식회사 비즈디알엠(전자상거래 사업자)가 운영하는 스마트업(이하 “사이트”라 한다)에서 제공하는 인터넷 관련
                    서비스(이하 “서비스”라 한다)를 이용함에 있어 온라인 사이트와 이용자의 권리.의무 및 책임사항을 규정함을 목적으로 합니다. ※「PC통신,
                    무선 등을 이용하는 전자상거래에 대해서도 그 성질에 반하지 않는제1조(목적) 이 약관은 주식회사 비즈디알엠(전자상거래 사업자)가
                    운영하는 스마트업(이하 “사이트”라 한다)에서 제공하는 인터넷 관련 서비스(이하 “서비스”라 한다)를 이용함에 있어 온라인 사이트와
                    이용자의 권리.의무 및 책임사항을 규정함을 목적으로 합니다. ※「PC통신, 무선 등을 이용하는 전자상거래에 대해서도 그 성질에 반하지
                    않는제1조(목적) 이 약관은 주식회사 비즈디알엠(전자상거래 사업자)가 운영하는 스마트업(이하 “사이트”라 한다)에서 제공하는 인터넷
                    관련 서비스(이하 “서비스”라 한다)를 이용함에 있어 온라인 사이트와 이용자의 권리.의무 및 책임사항을 규정함을 목적으로 합니다.
                    ※「PC통신, 무선 등을 이용하는 전자상거래에 대해서도 그 성질에 반하지 않는제1조(목적) 이 약관은 주식회사 비즈디알엠(전자상거래
                    사업자)가 운영하는 스마트업(이하 “사이트”라 한다)에서 제공하는 인터넷 관련 서비스(이하 “서비스”라 한다)를 이용함에 있어 온라인
                    사이트와 이용자의 권리.의무 및 책임사항을 규정함을 목적으로 합니다. ※「PC통신, 무선 등을 이용하는 전자상거래에 대해서도 그 성질에
                    반하지 않는
                  </div>
                </li>
                <li class="mb-4">
                  <div class="signup-check-box mb-3">
                    <input type="checkbox" name="" id="agreePrivacy" required />
                    <label class="flex items-center" for="agreePrivacy">
                      <span class="check-img"></span>
                      <span class="underline font-bold text-sm">개인정보 수집 및 이용 동의</span
                      ><small class="text-sm text-biz-red ml-px">(필수)</small></label
                    >
                  </div>
                  <div class="signup-content-box text-xs">
                    제1조(목적) 이 약관은 주식회사 비즈디알엠(전자상거래 사업자)가 운영하는 스마트업(이하 “사이트”라 한다)에서 제공하는 인터넷 관련
                    서비스(이하 “서비스”라 한다)를 이용함에 있어 온라인 사이트와 이용자의 권리.의무 및 책임사항을 규정함을 목적으로 합니다. ※「PC통신,
                    무선 등을 이용하는 전자상거래에 대해서도 그 성질에 반하지 않는 제1조(목적) 이 약관은 주식회사 비즈디알엠(전자상거래 사업자)가
                    운영하는 스마트업(이하 “사이트”라 한다)에서 제공하는 인터넷 관련 서비스(이하 “서비스”라 한다)를 이용함에 있어 온라인 사이트와
                    이용자의 권리.의무 및 책임사항을 규정함을 목적으로 합니다. ※「PC통신, 무선 등을 이용하는 전자상거래에 대해서도 그 성질에 반하지
                    않는 제1조(목적) 이 약관은 주식회사 비즈디알엠(전자상거래 사업자)가 운영하는 스마트업(이하 “사이트”라 한다)에서 제공하는 인터넷
                    관련 서비스(이하 “서비스”라 한다)를 이용함에 있어 온라인 사이트와 이용자의 권리.의무 및 책임사항을 규정함을 목적으로 합니다.
                    ※「PC통신, 무선 등을 이용하는 전자상거래에 대해서도 그 성질에 반하지 않는 제1조(목적) 이 약관은 주식회사 비즈디알엠(전자상거래
                    사업자)가 운영하는 스마트업(이하 “사이트”라 한다)에서 제공하는 인터넷 관련 서비스(이하 “서비스”라 한다)를 이용함에 있어 온라인
                    사이트와 이용자의 권리.의무 및 책임사항을 규정함을 목적으로 합니다. ※「PC통신, 무선 등을 이용하는 전자상거래에 대해서도 그 성질에
                    반하지 않는
                  </div>
                </li>
                <li class="mb-8">
                  <div class="signup-check-box mb-3">
                    <input type="checkbox" name="" id="agreePromotion" />
                    <label class="flex items-center" for="agreePromotion">
                      <span class="check-img"></span>
                      <span class="underline font-bold text-sm">프로모션 정보 수신 동의</span
                      ><small class="text-sm text-gray-92 ml-px">(선택)</small></label
                    >
                  </div>
                  <p class="text-xs">문자, 연락처, 이메일에 스마트업 서비스와 관련된 소식을 받아보겠습니다.</p>
                </li>
              </ul>
            </fieldset>
            <div class="flex justify-between gap-6">
              <a href="" class="inline-block w-full text-sm font-bold py-3 text-white text-center no-underline leading-none bg-biz-gray">취소</a>
              <button onclick="location.href='/login/signupForm'" class="w-full py-3 text-sm font-bold text-white bg-biz-red leading-none">
                확인
              </button>
            </div>
          </form>
        </div>
      </div>
</template>
