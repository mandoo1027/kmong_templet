<template>
    <div class="list-page bg-gray-f5">
        <div class="inner w-[90%] py-5 mx-auto lg:pt-[44px] lg:pb-[57px] lg:w-[90%] xl:w-[1200px]">
          <section>
            <h2 class="font-bold text-xl mb-3 flex justify-between lg:mb-4 lg:text-2xl">
              리스트
              <a
                href="/campaign/addList"
                class="inline-block no-underline py-2 p-3 text-sm font-bold rounded-md text-white bg-biz-red leading-none ml-25 lg:py-3 lg:px-6"
                >리스트추가</a
              >
            </h2>
            <div class="table-wrap table-responsive flex flex-col h-full bg-white justify-between mb-8 min-h-[300px] rounded-[11px] lg:min-h-[855px]">
              <table class="basic-table table table-hover table-borderless w-full">
                <thead>
                  <tr>
                    <th class="text-center" scope="col">#</th>
                    <th class="text-center" scope="col">리스트제목</th>
                    <th class="text-center" scope="col">리드</th>
                    <th class="text-center" scope="col">수정날짜</th>
                    <th class="text-center" scope="col">생성날짜</th>
                    <th class="text-center" scope="col">설정</th>
                  </tr>
                </thead>
                <tbody>
                  <tr>
                    <th class="text-center" scope="row">1</th>
                    <td class="text-center">잠재고객</td>
                    <td class="text-center">351</td>
                    <td class="text-center">2023-02-12 17:51</td>
                    <td class="text-center">2023-01-12 11:21</td>
                    <td class="text-center"><button type="button" class="setting"></button></td>
                  </tr>
                  <tr>
                    <th class="text-center" scope="row">2</th>
                    <td class="text-center">신규고객</td>
                    <td class="text-center">1,432</td>
                    <td class="text-center">2023-02-12 17:51</td>
                    <td class="text-center">2023-01-12 11:21</td>
                    <td class="text-center"><button type="button" class="setting"></button></td>
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
        </div>
      </div>
</template>
