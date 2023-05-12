<template>
 <div class="lead-page bg-gray-f5 pt-[50px] lg:pt-[44px] lg:pb-[66px]">
        <section class="w-[90%] lg:w-[90%] mx-auto xl:w-[1235px]">
          <h2 class="font-bold text-2xl mb-4 flex justify-between w-full lg:w-[605px]">
            리드
            <a
              href="/campaign/addLead"
              class="inline-block no-underline py-2 p-3 text-sm font-bold rounded-md text-white bg-biz-red leading-none ml-25 lg:py-3 lg:px-6"
              >리드추가</a
            >
          </h2>
          <div class="flex flex-col gap-8 xl:flex-row pb-5">
            <article class="bg-white rounded-t-lg overflow-hidden min-h-[300px] lg:min-h-[530px]">
              <h3 class="blind">표</h3>
              <div class="table-responsive flex flex-col h-full justify-between pb-4">
                <table class="basic-table table table-hover table-borderless">
                  <thead>
                    <tr>
                      <th class="text-center" scope="col">#</th>
                      <th class="text-left" scope="col">이메일</th>
                      <th class="text-center" scope="col">최종 수정일</th>
                      <th class="text-center" scope="col">설정</th>
                    </tr>
                  </thead>
                  <tbody>
                    <tr>
                      <th class="text-center" scope="row">1</th>
                      <td>jkhreel23@naver.com</td>
                      <td class="text-center">2023-02-12 17:51</td>
                      <td class="text-center"><button type="button" class="setting"></button></td>
                    </tr>
                    <tr>
                      <th class="text-center" scope="row">2</th>
                      <td>ejslkdn@gmail.com</td>
                      <td class="text-center">2023-02-12 17:51</td>
                      <td class="text-center"><button type="button" class="setting"></button></td>
                    </tr>
                    <tr>
                      <th class="text-center" scope="row">3</th>
                      <td>jkhreel23@naver.com</td>
                      <td class="text-center"></td>
                      <td class="text-center"><button type="button" class="setting"></button></td>
                    </tr>
                  </tbody>
                </table>
                <nav aria-label="Page navigation mt-auto">
                  <ul class="pagination justify-content-center gap-x-2">
                    <li class="page-item active"><a class="page-link" href="#">1</a></li>
                  </ul>
                  <!-- <ul class="pagination justify-content-center  gap-x-2">
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
              </div>
            </article>
            <article class="user-detail-info bg-white min-h-[300px] lg:min-h-[530px]">
              <h3 class="font-bold text-xl lg:text-2xl">jkhreel23@naver.com</h3>
              <ul class="nav nav-tabs nav-pills nav-fill" id="myTab" role="tablist">
                <li class="nav-item" role="presentation">
                  <button
                    class="nav-link active"
                    id="profile-tab"
                    data-bs-toggle="tab"
                    data-bs-target="#profile"
                    type="button"
                    role="tab"
                    aria-controls="profile"
                    aria-selected="true"
                  >
                    프로필
                  </button>
                </li>
                <li class="nav-item" role="presentation">
                  <button
                    class="nav-link"
                    id="activity-info-tab"
                    data-bs-toggle="tab"
                    data-bs-target="#activity-info"
                    type="button"
                    role="tab"
                    aria-controls="activity-info"
                    aria-selected="false"
                  >
                    활동정보
                  </button>
                </li>
                <li class="nav-item" role="presentation">
                  <button
                    class="nav-link"
                    id="list-tab"
                    data-bs-toggle="tab"
                    data-bs-target="#list"
                    type="button"
                    role="tab"
                    aria-controls="list"
                    aria-selected="false"
                  >
                    리스트
                  </button>
                </li>
              </ul>
              <div class="tab-content" id="myTabContent">
                <div class="tab-pane show active" id="profile" role="tabpanel" aria-labelledby="profile-tab">
                  <dl class="flex items-center">
                    <dt class="font-bold text-sm">이름</dt>
                    <dd class="text-sm">김현민</dd>
                  </dl>
                  <dl class="flex items-center">
                    <dt class="font-bold text-sm">전화번호</dt>
                    <dd class="text-sm">010-5462-0848</dd>
                  </dl>
                  <dl class="flex items-center">
                    <dt class="font-bold text-sm">성별</dt>
                    <dd class="text-sm">남</dd>
                  </dl>
                  <dl class="flex items-center">
                    <dt class="font-bold text-sm">회사</dt>
                    <dd class="text-sm">아이에이엠파트너즈</dd>
                  </dl>
                  <dl class="flex items-center">
                    <dt class="font-bold text-sm">생년월일</dt>
                    <dd class="text-sm">1996-02-12</dd>
                  </dl>
                  <dl class="flex items-center">
                    <dt class="font-bold text-sm">우편번호</dt>
                    <dd class="text-sm">06954</dd>
                  </dl>
                  <dl class="flex items-center">
                    <dt class="font-bold text-sm">주소</dt>
                    <dd class="text-sm">서울시 동작구 대방동 114-4</dd>
                  </dl>
                  <dl class="flex items-center">
                    <dt class="font-bold text-sm">상세주소</dt>
                    <dd class="text-sm"></dd>
                  </dl>
                  <dl class="flex items-center">
                    <dt class="font-bold text-sm">리드점수</dt>
                    <dd class="text-sm">12</dd>
                  </dl>
                </div>
                <div class="tab-pane fade" id="activity-info" role="tabpanel" aria-labelledby="activity-info-tab">활동정보</div>
                <div class="tab-pane fade" id="list" role="tabpanel" aria-labelledby="list-tab">리스트</div>
              </div>
            </article>
          </div>
        </section>
      </div>
</template>
