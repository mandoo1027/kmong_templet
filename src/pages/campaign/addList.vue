<template>
 <main class="bg-gray-f5">
      <div class="add-list-page">
        <div class="inner w-[90%] lg:w-[606px] py-[50px] mx-auto lg:pt-[83px] lg:pb-[153px]">
          <form action="">
            <fieldset>
              <legend class="text-center text-2xl font-bold mb-10">리스트 추가</legend>
              <ul>
                <li class="basic-input-wrap mb-12">
                  <label class="font-bold text-sm mb-[10px] lg:text-[14px]" for="userAdr2">리스트명</label>
                  <div class="flex">
                    <input
                      class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 lg:text-[14px] lg:px-[16px] lg:py-[11px]"
                      type="text"
                      id="userAdr2"
                      placeholder="리스트명을 입력해 주세요."
                    />
                  </div>
                </li>
              </ul>
            </fieldset>
            <div class="button-wrap flex justify-center gap-x-6">
              <a
                href="/campaign/list"
                class="inline-block rounded-md w-[100px] font-bold py-3 text-center no-underline text-sm leading-none bg-gray-d9 lg:w-[192px]"
                >취소</a
              >
              <a
                href="/campaign/list"
                class="inline-block rounded-md w-[100px] font-bold py-3 text-white text-center no-underline text-sm leading-none bg-biz-red lg:w-[192px]"
                >저장</a
              >
            </div>
          </form>
        </div>
      </div>
    </main>
</template>
