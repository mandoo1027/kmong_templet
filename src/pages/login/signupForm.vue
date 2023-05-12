 <template>
 <main class="bg-gray-f5">
      <div class="signup-page">
        <div class="w-[90%] lg:w-[384px] mx-auto pt-[60px] pb-[100px]">
          <figure class="logo">
            <img src="/assets/images/common/logo.svg" alt="BIZDRM" />
          </figure>
          <form action="">
            <fieldset>
              <legend class="text-center font-bold mb-20">비즈디알엠 회원가입</legend>
              <ul>
                <li class="mb-4">
                  <label class="font-bold text-sm mb-[10px] lg:text-[14px]" for="userId">아이디</label>
                  <div class="flex">
                    <input
                      type="text"
                      class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 lg:text-[14px] lg:px-[16px] lg:py-[11px]"
                      id="userId"
                      placeholder="영문+숫자 포함 최소 6자"
                      minlength="6"
                      required
                    />
                    <button class="check-button py-3 font-bold text-sm text-white bg-biz-red shrink-0 ml-[10px] leading-none" type="button">
                      중복확인
                    </button>
                  </div>
                  <p class="text-[12px] text-[#d10000] font-normal mt-[10px]">중복된 아이디 입니다.</p>
                </li>
                <li class="basic-input-wrap mb-4">
                  <label class="font-bold text-sm mb-[10px] lg:text-[14px]" for="userPwd1">비밀번호</label>
                  <div class="flex">
                    <input
                      class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 lg:text-[14px] lg:px-[16px] lg:py-[11px]"
                      type="password"
                      id="userPwd1"
                      placeholder="영문+숫자+특수문자 포함 최소 8자 이상"
                      minlength="8"
                      required
                    />
                  </div>
                  <p class="text-[12px] text-[#d10000] font-normal mt-[10px]">영문+숫자+특수문자 포함 최소 8자 이상으로 설정해 주세요.</p>
                </li>
                <li class="basic-input-wrap mb-8 lg:mb-16">
                  <label class="font-bold text-sm mb-[10px] lg:text-[14px]" for="userPwd2">비밀번호 확인</label>
                  <div class="flex">
                    <input
                      class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 lg:text-[14px] lg:px-[16px] lg:py-[11px]"
                      type="password"
                      id="userPwd2"
                      placeholder="비밀번호를 입력해 주세요."
                      minlength="8"
                      required
                    />
                  </div>
                  <p class="text-[12px] text-[#d10000] font-normal mt-[10px]">비밀번호가 일치하지 않습니다.</p>
                </li>
                <li class="basic-input-wrap mb-6">
                  <label class="font-bold text-sm mb-[10px] lg:text-[14px]" for="userName">이름</label>
                  <div class="flex">
                    <input
                      class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 lg:text-[14px] lg:px-[16px] lg:py-[11px]"
                      type="text"
                      id="userName"
                      placeholder="실명을 입력해 주세요."
                    />
                  </div>
                </li>
                <li class="basic-input-wrap mb-6">
                  <label class="font-bold text-sm mb-[10px] lg:text-[14px]" for="userBirth">생년월일</label>
                  <div class="flex">
                    <input
                      class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 lg:text-[14px] lg:px-[16px] lg:py-[11px]"
                      type="text"
                      inputmode="numeric"
                      id="userBirth"
                      placeholder="년(4자)"
                      minlength="4"
                    />
                    <select class="basic-select" name="" id="">
                      <option value="none">월</option>
                      <option value="1">1월</option>
                      <option value="2">2월</option>
                      <option value="3">3월</option>
                      <option value="4">4월</option>
                      <option value="5">5월</option>
                      <option value="6">6월</option>
                      <option value="7">7월</option>
                      <option value="8">8월</option>
                      <option value="9">9월</option>
                      <option value="10">10월</option>
                      <option value="11">11월</option>
                      <option value="12">12월</option>
                    </select>
                    <input
                      class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 lg:text-[14px] lg:px-[16px] lg:py-[11px]"
                      type="text"
                      inputmode="numeric"
                      id="userBirth"
                      placeholder="일"
                    />
                  </div>
                </li>
                <li class="basic-input-wrap mb-6">
                  <label class="font-bold text-sm mb-[10px] lg:text-[14px]" for="userEmail">본인확인 이메일</label>
                  <div class="flex">
                    <input
                      class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 lg:text-[14px] lg:px-[16px] lg:py-[11px]"
                      type="email"
                      id="userEmail"
                      placeholder="이메일을 입력해 주세요."
                    />
                  </div>
                </li>
                <li class="basic-input-wrap mb-16">
                  <label class="font-bold text-sm mb-[10px] lg:text-[14px]" for="userTel">휴대전화</label>
                  <div class="flex">
                    <input
                      class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 lg:text-[14px] lg:px-[16px] lg:py-[11px]"
                      type="text"
                      id="userTel"
                      placeholder="전화번호를 입력해 주세요."
                    />
                  </div>
                </li>
              </ul>
            </fieldset>
            <div class="flex justify-between gap-6">
              <button onclick="location.href='/login/signupComplete'" class="w-full py-3 text-sm font-bold text-white bg-biz-red leading-none">
                가입하기
              </button>
            </div>
          </form>
        </div>
      </div>
    </main>
    </template>