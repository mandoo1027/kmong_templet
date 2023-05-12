<template>
 <div class="campaign-page bg-biz-light-red">
    <div class="w-[90%] py-[50px] mx-auto xl:w-[1200px] xl:pt-[57px] xl:pb-[89px]">
      <ul class="flex flex-col gap-4 lg:flex-row">
        <li class="p-[15px] col bg-white rounded-md lg:pt-[28px] lg:pb-[24px] lg:px-[22px]">
          <form action="">
            <h2 class="text-biz-red font-bold text-center mb-4 text-lg xl:mb-8">캠페인 대상</h2>
            <ul>
              <li class="basic-input-wrap mb-6">
                <label class="font-bold text-sm mb-[10px] lg:text-[14px]" for="userApi">API Key</label>
                <div class="flex">
                  <input
                    class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 lg:text-[14px] lg:px-[16px] lg:py-[11px] rounded-md"
                    type="text"
                    id="userApi"
                    placeholder="API 키를 입력해 주세요."
                  />
                </div>
              </li>
              <li class="basic-input-wrap mb-4">
                <label class="font-bold text-sm mb-[10px] lg:text-[14px]" for="listId">List 아이디</label>
                <div class="flex">
                  <input
                    class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 lg:text-[14px] lg:px-[16px] lg:py-[11px] rounded-md"
                    type="text"
                    id="listId"
                    placeholder="List 아이디를 입력해 주세요."
                  />
                </div>
              </li>
            </ul>
            <div>
              <button class="w-full py-3 text-sm font-bold text-white bg-biz-red leading-none rounded-md">리스트 조회하기</button>
            </div>
          </form>
          <section class="mt-12">
            <h3 class="font-bold text-lg mb-3 flex flex-col justify-between gap-2 lg:flex-row lg:items-center">
              리드 목록
              <div class="flex gap-1">
                <button class="p-2 text-sm rounded-sm text-white bg-biz-purple leading-none font-normal" type="button">선택전송</button>
                <button class="p-2 text-sm rounded-sm text-white bg-biz-green leading-none ml-25 font-normal" type="button">
                  현재 페이지 전송
                </button>
                <button class="p-2 text-sm rounded-sm text-white bg-biz-red leading-none ml-25 font-normal" type="button">모두전송</button>
              </div>
            </h3>
            <div class="table-wrap table-responsive flex flex-col h-full bg-white justify-between mb-4">
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
                  <tr>
                    <th class="text-center" scope="row">
                      <div>
                        <input class="form-check-input" type="checkbox" id="checkboxNoLabel" value="" aria-label="..." />
                      </div>
                    </th>
                    <td class="text-center">afldkajfldkajfldak</td>
                    <td class="text-center">리드</td>
                  </tr>
                  <tr>
                    <th class="text-center" scope="row">
                      <div>
                        <input class="form-check-input" type="checkbox" id="checkboxNoLabel" value="" aria-label="..." />
                      </div>
                    </th>
                    <td class="text-center">afldkajfldkajfldak</td>
                    <td class="text-center">리드</td>
                  </tr>
                  <tr>
                    <th class="text-center" scope="row">
                      <div>
                        <input class="form-check-input" type="checkbox" id="checkboxNoLabel" value="" aria-label="..." />
                      </div>
                    </th>
                    <td class="text-center">afldkajfldkajfldak</td>
                    <td class="text-center">리드</td>
                  </tr>
                  <tr>
                    <th class="text-center" scope="row">
                      <div>
                        <input class="form-check-input" type="checkbox" id="checkboxNoLabel" value="" aria-label="..." />
                      </div>
                    </th>
                    <td class="text-center">afldkajfldkajfldak</td>
                    <td class="text-center">리드</td>
                  </tr>
                  <tr>
                    <th class="text-center" scope="row">
                      <div>
                        <input class="form-check-input" type="checkbox" id="checkboxNoLabel" value="" aria-label="..." />
                      </div>
                    </th>
                    <td class="text-center">afldkajfldkajfldak</td>
                    <td class="text-center">리드</td>
                  </tr>
                  <tr>
                    <th class="text-center" scope="row">
                      <div>
                        <input class="form-check-input" type="checkbox" id="checkboxNoLabel" value="" aria-label="..." />
                      </div>
                    </th>
                    <td class="text-center">afldkajfldkajfldak</td>
                    <td class="text-center">리드</td>
                  </tr>
                  <tr>
                    <th class="text-center" scope="row">
                      <div>
                        <input class="form-check-input" type="checkbox" id="checkboxNoLabel" value="" aria-label="..." />
                      </div>
                    </th>
                    <td class="text-center">afldkajfldkajfldak</td>
                    <td class="text-center">리드</td>
                  </tr>
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
            <nav aria-label="Page navigation">
              <ul class="pagination justify-content-center gap-x-2">
                <li class="page-item active"><a class="page-link" href="#">1</a></li>
              </ul>
              <!-- <ul class="pagination justify-content-center gap-x-2">
                <li class="page-item disabled">
                  <a class="page-link" href="#" tabindex="-1" aria-disabled="true"> <span aria-hidden="true">&laquo;</span></a>
                </li>
                <li class="page-item active"><a class="page-link" href="#">1</a></li>
                <li class="page-item"><a class="page-link" href="#">2</a></li>
                <li class="page-item"><a class="page-link" href="#">3</a></li>
                <li class="page-item">
                  <a class="page-link" href="#"><span aria-hidden="true">&raquo;</span></a>
                </li>
              </ul> -->
            </nav>
          </section>
        </li>
        <li class="p-[15px] col bg-white rounded-md lg:pt-[28px] lg:pb-[24px] lg:px-[22px]">
          <form action="">
            <h2 class="text-biz-red font-bold text-center mb-4 text-lg xl:mb-8">캠페인 설정</h2>
            <ul class="mb-3">
              <li class="form-check form-check-inline items-center">
                <input class="form-check-input" type="radio" name="connectSetting" id="msg" value="msg" />
                <label class="font-bold text-sm lg:text-[14px] form-check-label"   for="msg">문자</label>
              </li>
              <li class="form-check form-check-inline items-center">
                <input class="form-check-input" type="radio" name="connectSetting" id="email" value="email" />
                <label class="font-bold text-sm lg:text-[14px] form-check-label"   for="email">이메일</label>
              </li>
              <li class="form-check form-check-inline items-center">
                <input class="form-check-input" type="radio" name="connectSetting" id="both" value="both" checked />
                <label class="font-bold text-sm lg:text-[14px] form-check-label"   for="both">문자&이메일</label>
              </li>
            </ul>
            <ul>
              <li class="basic-input-wrap mb-6">
                <label class="font-bold text-sm mb-[10px] lg:text-[14px]" for="userApi">메세지 유형 선택</label>
                <div class="flex">
                  <select class="basic-select" name="" id="">
                    <option value="1">자동응답</option>
                    <option value="2">자동응답2</option>
                    <option value="3">자동응답3</option>
                  </select>
                </div>
              </li>
              <li class="basic-input-wrap mb-4">
                <label class="font-bold text-sm mb-[10px] lg:text-[14px]" for="listId">서비스 명 입력</label>
                <div class="flex">
                  <input
                    class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 lg:text-[14px] lg:px-[16px] lg:py-[11px]"
                    type="text"
                    id="listId"
                    placeholder="메세지에 들어갈 서비스 명을 입력하세요."
                  />
                </div>
              </li>
              <li class="basic-input-wrap mb-4">
                <label class="font-bold text-sm mb-[10px] lg:text-[14px]" for="listId">URL 입력</label>
                <div class="flex">
                  <input
                    class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 lg:text-[14px] lg:px-[16px] lg:py-[11px]"
                    type="text"
                    id="listId"
                    placeholder="메세지에 들어갈 홈페이지 URL을 입력하세요."
                  />
                </div>
              </li>
              <li class="basic-input-wrap mb-12">
                <label class="font-bold text-sm mb-[10px] lg:text-[14px]" for="listId">메시지 API Key 입력</label>
                <div class="flex">
                  <input
                    class="w-full bg-white border-solid border-gray-d9 text-sm px-2.5 py-2.5 border-1 lg:text-[14px] lg:px-[16px] lg:py-[11px]"
                    type="text"
                    id="listId"
                    placeholder="메시지 발송 API Key를 입력해 주세요."
                  />
                </div>
                <p class="text-[12px] text-[#d10000] font-normal mt-[10px]">메세지는 API 연동으로 전송됩니다.</p>
              </li>
            </ul>
            <div>
              <button class="w-full py-3 text-sm font-bold text-white bg-biz-red leading-none rounded-md">메세지 전송</button>
            </div>
          </form>
        </li>
        <li class="p-[15px] col bg-white rounded-md lg:pt-[28px] lg:pb-[24px] lg:px-[22px]">
          <h2 class="text-biz-red font-bold text-center text-lg mb-4 text-lg xl:mb-12">전송 문자 & 메일 샘플 미리보기</h2>
          <div class="sample-box border leading-normal text-sm">
            <span class="text-biz-blue">[이름]</span>님,<br />
            <span class="text-biz-blue">[서비스 명]</span>쿠폰 이벤트에 신청해 주셔서 감사합니다.<br />
            이용방법 및 기타 문의는 메세지 남겨 주시면 연락 드리겠습니다.<br />
            <br />
            ► 더 알아보기<br />
            <span class="text-biz-blue">[홈페이지 URL]</span><br />
            <br />
            감사합니다.<br />
          </div>
          <p class="text-sm leading-normal text-[#777777] mt-7">
            ※ [ ]사이 내용은 캠페인 설정에 따라 자동으로 입력됩니다.<br />
            <br />
            ※ 지나치게 긴 내용이나 반복된 메세지는 스팸차단 될 수 있으므로, 300자 내외로 작성하는 것을 권장드립니다.
          </p>
        </li>
      </ul>
    </div>
  </div>
</template>
