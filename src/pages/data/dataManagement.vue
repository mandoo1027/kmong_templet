<template>
  <div class="data-management-page bg-biz-light-red">
        <div class="bg-[#822325] xl:h-[277px]">
          <div class="w-[90%] mx-auto h-full xl:w-[1200px]">
            <ul class="flex flex-col h-full xl:flex-row">
              <li class="shrink-0 w-full flex items-center py-3 justify-center xl:w-[385px] xl:py-0">
                <h2 class="text-white font-bold text-[28px]">Data Query</h2>
              </li>
              <li class="shrink-0 flex flex-col items-center gap-5 pb-5 xl:gap-16 w-full mx-auto xl:flex-row xl:flex-1 xl:pb-0 xl:gap-2">
                <ul class="w-full xl:ml-auto xl:flex-0 xl:w-auto">
                  <li class="flex mb-2 items-center w-full xl:mb-6 xl:w-auto">
                    <label class="w-[120px] shrink-0 text-white text-sm font-bold xl:w-[102px] xl:pl-2" for="">검색한 리스트명</label>
                    <div class="w-full xl:w-[330px]">
                      <input
                        id="listName"
                        class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 xl:text-[14px] xl:px-[16px] xl:py-[11px]"
                        type="text"
                        placeholder="리스트명"
                      />
                    </div>
                  </li>
                  <li class="flex mb-2 items-center w-full xl:mb-6 xl:w-auto">
                    <label class="w-[120px] shrink-0 text-white text-sm font-bold xl:w-[102px] xl:pl-2" for="">리스트 아이디</label>
                    <div class="w-full xl:w-[330px]">
                      <input
                        id="listId"
                        class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 xl:text-[14px] xl:px-[16px] xl:py-[11px]"
                        type="text"
                        placeholder="리스트 아이디"
                      />
                    </div>
                  </li>
                  <li class="flex items-center w-full xl:w-auto">
                    <label class="w-[120px] shrink-0 text-white text-sm font-bold xl:w-[102px] xl:pl-2" for="">API Key</label>
                    <div class="w-full xl:w-[330px]">
                      <input
                        id="apiKey"
                        class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 xl:text-[14px] xl:px-[16px] xl:py-[11px]"
                        type="text"
                        placeholder="API Key"
                      />
                    </div>
                  </li>
                </ul>
                <button
                  class="shrink-0 w-[300px] h-fit p-2 bg-[#BE3034] rounded-xl flex items-center justify-center xl:flex-col xl:p-0 xl:w-[131px] xl:h-[125px]"
                >
                  <span class="search-img shrink-0 order-2 xl:order-1 w-[20px] h-[20px] xl:w-[38px] xl:h-[38px]"></span>
                  <span class="text-white font-bold text-base mr-2 order-1 xl:mt-2.5 xr:ml-0 xl:order-2">리스트 조회</span>
                </button>
              </li>
            </ul>
          </div>
        </div>
        <div class="w-[90%] mx-auto h-full xl:w-[1200px]">
          <div class="py-8 xl:py-24">
            <ul class="flex flex-col gap-4 xl:flex-row">
              <li class="flex-1 bg-white rounded-md p-[15px] xl:py-[30px] xl:px-[25px] min-h-[200px]">
                <h2 class="font-bold text-lg mb-8">리스트 목록</h2>
              </li>
              <li class="flex-1 bg-white rounded-md p-[15px] xl:py-[30px] xl:px-[25px] min-h-[200px]">
                <h2 class="blind">리드, 방문자 목록</h2>
                <section class="mb-5">
                  <h3 class="font-bold text-lg mb-3 flex flex-col justify-between gap-2 lg:flex-row lg:items-center">
                    리드 목록
                    <div class="flex gap-1">

                   
                      <button  class="p-2 text-sm rounded-sm text-white bg-biz-purple leading-none font-normal" >선택저장</button>
                      <button class="p-2 text-sm rounded-sm text-white bg-biz-green leading-none ml-25 font-normal" >
                        현재 페이지 저장
                      </button>
                      <button class="p-2 text-sm rounded-sm text-white bg-biz-red leading-none ml-25 font-normal">모두저장</button>
                    </div>
                  </h3>
                  <div class="table-wrap table-responsive flex flex-col bg-white justify-between h-60">
                    <table class="red-table table table-borderless table-striped mb-0">
                      <thead>
                        <tr>
                          <th class="text-center" colspan="3">리드코드</th>
                        </tr>
                      </thead>
                      <tbody>
                        <tr>
                          <th class="text-center" scope="row">
                            <div>
                              <input class="form-check-input" type="checkbox" id="checkboxNoLabel" value="" aria-label="..." />
                            </div>
                          </th>
                          <td class="text-center">afldkajfldkajfldak</td>
                          <td class="text-center">리드</td>
                        </tr>
                      </tbody>
                    </table>
                  </div>
                </section>
                <section class="">
                  <h3 class="font-bold text-lg mb-2.5 flex flex-col justify-between gap-2 lg:flex-row lg:items-center">
                    방문자 목록
                    <div class="flex gap-1">
                      <button class="p-2 text-sm rounded-sm text-white bg-biz-purple leading-none font-normal">선택저장</button>
                      <button class="p-2 text-sm rounded-sm text-white bg-biz-green leading-none ml-25 font-normal" >
                        현재 페이지 저장
                      </button>
                      <button class="p-2 text-sm rounded-sm text-white bg-biz-red leading-none ml-25 font-normal" >모두저장</button>
                    </div>
                  </h3>
                  <div class="table-wrap table-responsive flex flex-col bg-white justify-between h-60">
                    <table class="red-table table table-borderless table-striped mb-0">
                      <thead>
                        <tr>
                          <th class="text-center" colspan="3">방문자 코드</th>
                        </tr>
                      </thead>
                      <tbody>
                        <tr>
                          <th class="text-center" scope="row">
                            <div>
                              <input class="form-check-input" type="checkbox" id="checkboxNoLabel" value="" aria-label="..." />
                            </div>
                          </th>
                          <td class="text-center">text</td>
                          <td class="text-center">text</td>
                        </tr>
                        <tr>
                          <th class="text-center" scope="row">
                            <div>
                              <input class="form-check-input" type="checkbox" id="checkboxNoLabel" value="" aria-label="..." />
                            </div>
                          </th>
                          <td class="text-center">text</td>
                          <td class="text-center">text</td>
                        </tr>
                      </tbody>
                    </table>
                  </div>
                </section>
              </li>
              <li class="flex-1 bg-white rounded-md p-[15px] xl:py-[30px] xl:px-[25px] min-h-[200px]">
                <h2 class="font-bold text-lg mb-12">이벤트 목록</h2>
              </li>
            </ul>
          </div>
        </div>
      </div>
</template>
