<template>
 <div class="dashboard-page bg-biz-light-red flex flex-col xl:flex-row">
        <nav class="dashboard-nav w-full bg-[#543438] p-3 xl:py-10 xl:w-[380px]">
          <button
            class="text-base flex items-center text-white justify-between w-full text-center font-bold xl:hidden"
            type="button"
            onclick="Toggle(this)"
          >
            <span>서브메뉴</span>
            <svg data-accordion-icon class="w-6 h-6 shrink-0 ml-auto" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
              <path
                fill-rule="evenodd"
                d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                clip-rule="evenodd"
              ></path>
            </svg>
          </button>
          <ul class="hidden w-full mt-3 xl:w-[263px] xl:ml-auto xl:mt-0 xl:block">
            <li>
              <p class="flex items-center mb-2.5 pl-10">
                <span class="chart-icon w-[27px] h-[27px] shrink-0"></span>
                <span class="text-white text-base ml-[17px]">통계</span>
              </p>
              <ul class="nav nav-tabs flex-col border-0" id="myTab" role="tablist">
                <li class="nav-item" role="presentation">
                  <button
                    class="nav-link flex items-center w-full text-white border-0 text-left text-sm active"
                    id="all-chart-tab"
                    data-bs-toggle="tab"
                    data-bs-target="#all-chart"
                    type="button"
                    role="tab"
                    aria-controls="all-chart"
                    aria-selected="true"
                  >
                    전체 통계
                  </button>
                </li>
                <li class="nav-item" role="presentation">
                  <button
                    class="nav-link flex items-center w-full text-white border-0 text-left text-sm"
                    id="daily-reprot-tab"
                    data-bs-toggle="tab"
                    data-bs-target="#daily-reprot"
                    type="button"
                    role="tab"
                    aria-controls="daily-reprot"
                    aria-selected="false"
                  >
                    Daily Report
                  </button>
                </li>
                <li class="nav-item" role="presentation">
                  <button
                    class="nav-link flex items-center w-full text-white border-0 text-left text-sm"
                    id="list-tab"
                    data-bs-toggle="tab"
                    data-bs-target="#compare"
                    type="button"
                    role="tab"
                    aria-controls="compare"
                    aria-selected="false"
                  >
                    캠페인 성과 비교하기
                  </button>
                </li>
              </ul>
            </li>
            <li class="mt-4">
              <button class="flex items-center pl-10">
                <span class="excel-icon w-[36px] h-[36px] shrink-0"></span>
                <span class="text-white text-base ml-[17px]">엑셀 다운로드</span>
              </button>
            </li>
            <li class="mt-9">
              <div class="bg-white rounded-md border-2 border-[#F14A4A] py-2 xl:mr-[17px]">
                <ul class="flex justify-center gap-[29px]">
                  <li class="flex flex-col items-center">
                    <p class="leading-[1.87] text-sm">520 명</p>
                    <div class="relative bg-[#c0a6a7] rounded-md h-[100px] w-[20px] lx:h-[134px] lx:w-[36px]">
                      <span class="absolute bottom-0 w-[20px] bg-[#aa2024] rounded-md lx:w-[36px]" style="height: 20px"></span>
                    </div>
                    <label for="lead" class="leading-[1.87] text-sm mt-[7px]">LEAD</label>
                  </li>
                  <li class="flex flex-col items-center">
                    <p class="leading-[1.87] text-sm">2800 회</p>
                    <div class="relative bg-[#c0a6a7] rounded-md h-[100px] w-[20px] lx:h-[134px] lx:w-[36px]">
                      <span class="absolute bottom-0 w-[20px] bg-[#aa2024] rounded-md lx:w-[36px]" style="height: 80px"></span>
                    </div>
                    <label for="advertising" class="leading-[1.87] text-sm mt-[7px]">광고노출</label>
                  </li>
                </ul>
                <p class="text-[#E91C36] font-bold text-sm leading-[1.87] mt-px text-center">SPECIAL PLAN</p>
              </div>
            </li>
          </ul>
        </nav>
        <!-- CONTENT -->
        <div class="tab-content flex-1" id="myTabContent">
          <!-- 1. 전체 통계 -->
          <div class="tab-pane show active" id="all-chart" role="tabpanel" aria-labelledby="all-chart-tab">
            <div class="w-[90%] mx-auto py-[15px] xl:w-[1060px] xl:pt-[28px] xl:px-[34px] xl:pb-[49px] xl:p-[15px]">
              <select class="basic-select w-full px-[15px] py-[10px] border-[#AA2024] xl:w-[275px] xl:px-[26px] xl:py-[13px]" name="" id="">
                <option value="1">캠페인 이름 노출되는 곳</option>
                <option value="2">캠페인 이름 노출되는 곳2</option>
                <option value="3">캠페인 이름 노출되는 곳3</option>
                <option value="4">캠페인 이름 노출되는 곳4</option>
              </select>
              <ul class="campaign-visit-click-graph flex flex-col gap-4 mt-[29px] mb-[23px] xl:flex-row">
                <li class="w-full xl:w-[650px]">
                  <div class="flex flex-col justify-between mb-[11px] xl:flex-row">
                    <p class="text-base font-bold">캠페인 방문, 클릭 수 추이</p>
                    <ul class="nav nav-tabs nav-pills nav-fill mt-2 xl:mt-0" id="myTab" role="tablist">
                      <li class="nav-item" role="presentation">
                        <button
                          class="nav-link"
                          id="clickValue-tab"
                          data-bs-toggle="tab"
                          data-bs-target="#clickValue"
                          type="button"
                          role="tab"
                          aria-controls="clickValue"
                          aria-selected="false"
                        >
                          클릭 수 보기
                        </button>
                      </li>
                      <li class="nav-item" role="presentation">
                        <button
                          class="nav-link active"
                          id="visitsValue-tab"
                          data-bs-toggle="tab"
                          data-bs-target="#visitsValue"
                          type="button"
                          role="tab"
                          aria-controls="visitsValue"
                          aria-selected="true"
                        >
                          방문 수 보기
                        </button>
                      </li>
                    </ul>
                  </div>
                  <div class="tab-content bg-white rounded-lg p-4 h-[200px] xl:h-[376px]" id="Graph">
                    <div class="tab-pane h-full fade" id="clickValue" ro le="tabpanel" aria-labelledby="clickValue-tab">
                      <div class="w-full h-full flex">
                        <canvas id="" class="mt-auto"></canvas>
                      </div>
                    </div>
                    <div class="tab-pane h-full show active" id="visitsValue" role="tabpanel" aria-labelledby="visitsValue-tab">
                      <div class="w-full h-full flex">
                        <canvas id="CampaignLineGraph" class="mt-auto"></canvas>
                      </div>
                    </div>
                  </div>
                </li>
                <li class="flex-1">
                  <div class="calendar-box bg-white w-full rounded-lg p-4 lg:mt-[47px]">
                    <div class="h-full" id="calendar"></div>
                  </div>
                </li>
              </ul>
              <ul class="flex flex-wrap pt-[23px] gap-x-[2%]">
                <li class="shrink-0 w-[49%] xl:w-[23.5%]">
                  <p class="text-base font-bold mb-[11px]">누적 캠페인 방문 수</p>
                  <div class="flex items-center rounded-md red-gradient px-[23px] h-[105px]">
                    <p class="flex flex-col">
                      <b class="text-white font-bold text-lg">321명</b>
                      <span class="text-white text-base mt-[2px]">전체 80.2%</span>
                    </p>
                  </div>
                </li>
                <li class="shrink-0 w-[49%] xl:w-[23.5%]">
                  <p class="text-base font-bold mb-[11px]">누적 버튼 클릭 수</p>
                  <div class="flex items-center rounded-md red-gradient px-[23px] h-[105px]">
                    <p class="flex flex-col">
                      <b class="text-white font-bold text-lg">159명</b>
                      <span class="text-white text-base mt-[2px]">전체 52.2%</span>
                    </p>
                  </div>
                </li>
                <li class="shrink-0 w-[49%] mt-[20px] xl:w-[23.5%] xl:mt-0">
                  <p class="text-base font-bold mb-[11px]">캠페인 평균 체류 시간</p>
                  <div class="flex items-center rounded-md red-gradient px-[23px] h-[105px]">
                    <p>
                      <b class="text-white font-bold text-lg">3분</b>
                    </p>
                  </div>
                </li>
                <li class="shrink-0 w-[49%] mt-[20px] xl:w-[23.5%] xl:mt-0">
                  <p class="text-base font-bold mb-[11px]">평균 PV(Page View)</p>
                  <div class="flex items-center rounded-md red-gradient px-[23px] h-[105px]">
                    <p>
                      <b class="text-white font-bold text-lg">15페이지</b>
                    </p>
                  </div>
                </li>
              </ul>
              <ul class="flex flex-col pt-[23px] gap-4 xl:flex-row xl:mt-[26px]">
                <li class="flex-1 py-2">
                  <p class="text-base font-bold mb-[11px]">이탈률 추이</p>
                  <div class="bg-white w-full rounded-lg p-4">
                    <canvas id="DeviationRateTrendLine"></canvas>
                  </div>
                </li>
                <li class="flex-1 py-2">
                  <p class="text-base font-bold mb-[11px]">캠페인 체류시간 추이</p>
                  <div class="bg-white w-full rounded-lg p-4">
                    <canvas id="TimeOfStayLine"></canvas>
                  </div>
                </li>
              </ul>
              <ul class="flex flex-col pt-[23px] xl:flex-row xl:mt-[26px]">
                <li class="w-full py-2 xl:w-[49%]">
                  <p class="text-base font-bold mb-[11px]">유입 경로</p>
                  <div class="bg-white w-full rounded-lg flex p-4">
                    <div class="relative w-[125px]">
                      <p class="doughnut-value">100%</p>
                      <canvas id="VisitRoute"></canvas>
                    </div>
                    <ul class="ml-[26px] flex flex-col justify-center flex-1 gap-2">
                      <li class="flex items-center justify-between">
                        <p class="flex items-center">
                          <span class="w-[8px] h-[8px] rounded-[50%] shrink-0 bg-[#AA2024] mr-[13px]"></span>
                          <span class="text-sm">문자</span>
                        </p>
                        <span class="text-sm font-bold">60%</span>
                      </li>
                      <li class="flex items-center justify-between">
                        <p class="flex items-center">
                          <span class="w-[8px] h-[8px] rounded-[50%] shrink-0 bg-[#4250D8] mr-[13px]"></span>
                          <span class="text-sm">이메일</span>
                        </p>
                        <span class="text-sm font-bold">30%</span>
                      </li>
                      <li class="flex items-center justify-between">
                        <p class="flex items-center">
                          <span class="w-[8px] h-[8px] rounded-[50%] shrink-0 bg-[#D9D9D9] mr-[13px]"></span>
                          <span class="text-sm">기타</span>
                        </p>
                        <span class="text-sm font-bold">10%</span>
                      </li>
                    </ul>
                  </div>
                </li>
              </ul>
            </div>
          </div>
          <!-- 2. Daily Report -->
          <div class="tab-pane fade" id="daily-reprot" role="tabpanel" aria-labelledby="daily-reprot-tab">Daily Report</div>
          <!-- 3. 캠페인 성과 비교 -->
          <div class="tab-pane fade" id="compare" role="tabpanel" aria-labelledby="compare-tab">캠페인 성과 비교하기</div>
        </div>
      </div>
</template>


 <script>
      const CampaignLineChart = document.getElementById("CampaignLineGraph");
      let campaignVisitData = {
        labels: [
          "1",
          "2",
          "3",
          "4",
          "5",
          "6",
          "7",
          "8",
          "9",
          "10",
          "11",
          "12",
          "13",
          "14",
          "15",
          "16",
          "17",
          "18",
          "19",
          "20",
          "21",
          "22",
          "23",
          "24",
          "25",
          "26",
          "27",
          "28",
          "29",
          "30",
          "31",
        ],
        datasets: [
          {
            label: "방문 수 보기",
            data: [65, 59, 80, 81, 26, 55, 40, 65, 59, 80, 65, 59, 80, 81, 26, 55, 40, 65, 59, 80, 65, 59, 80, 81, 26, 55, 40, 65, 59, 80, 300],
            borderWidth: 2, // 선 굵기
            borderColor: "#AA2024",
            pointBorderWidth: 0,
            tension: 0.3,
          },
        ],
      };

      new Chart(CampaignLineChart, {
        type: "line",
        data: campaignVisitData,
        options: {
          scales: {
            y: {
              // defining min and max so hiding the dataset does not change scale range
              min: 0,
              max: 350,
              grid: {
                drawBorder: false,
              },
            },
            x: {
              grid: {
                display: false,
              },
            },
          },
          plugins: {
            legend: false,
          },
        },
      });
    </script>
    <script>
      const DeviationRateTrendLineChart = document.getElementById("DeviationRateTrendLine");
      let DeviationRateTrendLineData = {
        labels: ["3-1", "3-3", "3-6", "3-9", "3-15", "3-16"],
        datasets: [
          {
            label: "이탈률 추이",
            data: [60, 30, 40, 55, 30, 20],
            fill: false,
            borderWidth: 2, // 선 굵기
            borderColor: "#700CAE",
            pointBorderWidth: 0,
            tension: 0.3,
          },
        ],
      };

      new Chart(DeviationRateTrendLineChart, {
        type: "line",
        data: DeviationRateTrendLineData,
        options: {
          scales: {
            y: {
              min: 0,
              max: 100,
            },
            x: {
              grid: {
                display: false,
              },
            },
          },
          plugins: {
            legend: false,
            tooltip: {
              // 기존 툴팁 사용 안 함
              enabled: false,
            },
          },
        },
      });
    </script>
    <script>
      const TimeOfStayLineChart = document.getElementById("TimeOfStayLine");
      let TimeOfStayLineData = {
        labels: ["3-1", "3-3", "3-6", "3-9", "3-15", "3-16"],
        datasets: [
          {
            label: "캠페인 체류시간 추이",
            data: [60, 30, 40, 55, 30, 20],
            fill: false,
            borderWidth: 2, // 선 굵기
            borderColor: "#0CAEA4",
            pointBorderWidth: 0,
            tension: 0.3,
          },
        ],
      };

      new Chart(TimeOfStayLineChart, {
        type: "line",
        data: TimeOfStayLineData,
        options: {
          scales: {
            y: {
              min: 0,
              max: 100,
            },
            x: {
              grid: {
                display: false,
              },
            },
          },
          plugins: {
            legend: false,
            tooltip: {
              // 기존 툴팁 사용 안 함
              enabled: false,
            },
          },
        },
      });
    </script>
    <script>
      const VisitDoughnut = document.getElementById("VisitRoute");

      new Chart(VisitDoughnut, {
        type: "doughnut",
        data: {
          labels: ["문자", "이메일", "기타"],
          datasets: [
            {
              label: "유입 경로",
              data: [60, 30, 10],
              borderWidth: 1,
              backgroundColor: ["#AA2024", "#4250D8", "#D9D9D9"],
              hoverOffset: 4,
            },
          ],
        },
        options: {
          events: [],
          cutout: 40, //   도넛 width 값 수정
          plugins: {
            legend: {
              display: false,
            },
            labels: {
              font: {
                size: 14,
                family: "Pretendard",
              },
            },
          },
        },
      });
    </script>
    <script>
      document.addEventListener("DOMContentLoaded", function () {
        var calendarEl = document.getElementById("calendar");
        var calendar = new FullCalendar.Calendar(calendarEl, {
          initialView: "dayGridMonth",
        });
        calendar.render();
      });
    </script>
