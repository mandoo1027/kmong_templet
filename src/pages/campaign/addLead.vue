<template>
  <main class="bg-gray-f5">
      <div class="add-lead-page">
        <div class="inner w-[90%] lg:w-[606px] py-[50px] mx-auto lg:pt-[42px] lg:pb-[48px]">
          <form action="">
            <fieldset>
              <legend class="text-center text-2xl font-bold mb-10">리드추가</legend>
              <ul>
                <li class="basic-input-wrap flex flex-col gap-x-10 mb-2.5 lg:mb-8 lg:flex-row">
                  <div class="flex-1">
                    <label class="font-bold text-sm mb-[10px] lg:text-[14px]" for="userName">이름</label>
                    <div class="flex">
                      <input
                        class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 lg:text-[14px] lg:px-[16px] lg:py-[11px]"
                        type="text"
                        id="userName"
                        placeholder="이름을 입력해 주세요."
                      />
                    </div>
                  </div>
                  <div class="flex-1 mt-2.5 lg:mt-0">
                    <label class="font-bold text-sm mb-[10px] lg:text-[14px]" for="userGender">성별</label>
                    <div class="flex">
                      <div class="radio-box flex-1">
                        <input
                          class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 lg:text-[14px] lg:px-[16px] lg:py-[11px]"
                          type="radio"
                          id="female"
                          name="gender"
                          checked
                        />
                        <label class="font-bold text-sm mb-[10px] leading-none lg:text-[14px]" for="female">여성</label>
                      </div>
                      <div class="radio-box flex-1">
                        <input
                          class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 lg:text-[14px] lg:px-[16px] lg:py-[11px]"
                          type="radio"
                          id="male"
                          name="gender"
                        />
                        <label class="font-bold text-sm mb-[10px] leading-none lg:text-[14px]" for="male">남성</label>
                      </div>
                    </div>
                  </div>
                </li>
                <li class="basic-input-wrap flex flex-col gap-x-10 mb-2.5 lg:mb-8 lg:flex-row">
                  <div class="flex-1">
                    <label class="font-bold text-sm mb-[10px] lg:text-[14px]" for="userAge">나이</label>
                    <div class="flex">
                      <input
                        class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 lg:text-[14px] lg:px-[16px] lg:py-[11px]"
                        type="text"
                        id="userAge"
                        inputmode="numeric"
                        placeholder="나이를 입력해 주세요."
                      />
                    </div>
                  </div>
                  <div class="flex-1 mt-2.5 lg:mt-0">
                    <label class="font-bold text-sm mb-[10px] lg:text-[14px]" for="userTel">전화번호</label>
                    <div class="flex">
                      <input
                        class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 lg:text-[14px] lg:px-[16px] lg:py-[11px]"
                        type="text"
                        id="userTel"
                        placeholder="010-0000-0000"
                      />
                    </div>
                  </div>
                </li>
                <li class="basic-input-wrap flex flex-col gap-x-10 mb-2.5 lg:mb-8 lg:flex-row">
                  <div class="flex-1">
                    <label class="font-bold text-sm mb-[10px] lg:text-[14px]" for="userBirth">생년월일</label>
                    <div class="flex">
                      <input
                        class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 lg:text-[14px] lg:px-[16px] lg:py-[11px]"
                        type="text"
                        id="userBirth"
                        placeholder="YYYY-MM-DD"
                      />
                    </div>
                  </div>
                  <div class="flex-1 mt-2.5 lg:mt-0">
                    <label class="font-bold text-sm mb-[10px] lg:text-[14px]" for="userCompany">회사명</label>
                    <div class="flex">
                      <input
                        class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 lg:text-[14px] lg:px-[16px] lg:py-[11px]"
                        type="text"
                        id="userCompany"
                        placeholder="회사명을 입력해 주세요."
                      />
                    </div>
                  </div>
                </li>
                <li class="basic-input-wrap mb-2.5 lg:mb-8">
                  <label class="font-bold text-sm mb-[10px] lg:text-[14px]" for="userEmail">이메일</label>
                  <div class="flex">
                    <input
                      class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 lg:text-[14px] lg:px-[16px] lg:py-[11px]"
                      type="email"
                      id="userEmail"
                      placeholder="example@domain.com"
                    />
                  </div>
                </li>
                <li class="basic-input-wrap mb-2.5 lg:mb-8">
                  <label class="font-bold text-sm mb-[10px] lg:text-[14px]" for="userAdrNum">우편번호</label>
                  <div class="flex">
                    <input
                      class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 lg:text-[14px] lg:px-[16px] lg:py-[11px]"
                      type="text"
                      id="userAdrNum"
                      placeholder="우편번호를 입력해 주세요."
                      readonly
                    />
                    <button class="find-address-button py-3 font-bold text-sm text-white bg-biz-red leading-none" type="button">우편번호 검색</button>
                  </div>
                </li>
                <li class="basic-input-wrap mb-2.5 lg:mb-8">
                  <label class="font-bold text-sm mb-[10px] lg:text-[14px]" for="userAdr1">주소1</label>
                  <div class="flex">
                    <input
                      class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 lg:text-[14px] lg:px-[16px] lg:py-[11px]"
                      type="text"
                      id="userAdr1"
                      placeholder="주소를 입력해 주세요."
                    />
                  </div>
                </li>
                <li class="basic-input-wrap mb-6 lg:mb-12">
                  <label class="font-bold text-sm mb-[10px] lg:text-[14px]" for="userAdr2">주소2</label>
                  <div class="flex">
                    <input
                      class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 lg:text-[14px] lg:px-[16px] lg:py-[11px]"
                      type="text"
                      id="userAdr2"
                      placeholder="주소를 입력해 주세요."
                    />
                  </div>
                </li>
              </ul>
            </fieldset>
            <div class="button-wrap flex justify-center gap-x-6">
              <a
                href="/campaign/lead"
                class="inline-block rounded-md w-[100px] font-bold py-3 text-center no-underline text-sm leading-none bg-gray-d9 lg:w-[192px]"
                >취소</a
              >
              <a
                href="/campaign/lead"
                class="inline-block rounded-md w-[100px] font-bold py-3 text-white text-center no-underline text-sm leading-none bg-biz-red lg:w-[192px]"
                >저장</a
              >
            </div>
          </form>
        </div>
      </div>
    </main>
</template>
