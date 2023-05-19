<template>
  <header class="bg-white sticky shadow-sm top-0 z-20 xl:h-[74px]">
    <!-- PC 네비게이션 -->
    <nav
      class="relative h-full w-full flex justify-between items-center bg-white mx-auto xl:p-0 xl:w-[1200px]"
    >
      <a class="p-0 flex-shrink-0 leading-none" href="/main/main">
        <div class="logo"></div>
      </a>
      <div class="xl:hidden">
        <button
          @click="toggleButton"
          class="navbar-burger flex items-center text-biz-red p-3"
        >
          <svg
            class="block h-4 w-4 fill-current"
            viewBox="0 0 20 20"
            xmlns="http://www.w3.org/2000/svg"
          >
            <title>Mobile menu</title>
            <path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"></path>
          </svg>
        </button>
      </div>
      <ul
        class="hidden xl:flex xl:ml-auto xl:flex xl:items-center xl:w-auto xl:space-x-[45px] h-full"
      >
        <li>
          <a
            class="nav-link px-0 relative flex items-center font-bold hover:text-biz-red text-[16px] text-center text-[#454545] h-[74px]"
            href="/main/main"
            >HOME</a
          >
        </li>
        <li>
          <a
            class="nav-link px-0 relative flex items-center font-bold hover:text-biz-red text-[16px] text-center text-[#454545] h-[74px]"
            href="#"
            >서비스 소개</a
          >
        </li>
        <li>
          <a
            class="nav-link px-0 relative flex items-center font-bold hover:text-biz-red text-[16px] text-center text-[#454545] h-[74px]"
            href="#"
            >고객지원</a
          >
        </li>
        <li>
          <a
            class="nav-link px-0 relative flex items-center font-bold hover:text-biz-red text-[16px] text-center text-[#454545] h-[74px]"
            href="/data/dataManagement"
            >데이터 관리</a
          >
        </li>
        <li class="nav-item relative">
          <a
            class="nav-link px-0 relative flex items-center font-bold hover:text-biz-red text-[16px] text-center text-[#454545] h-[74px]"
            href="/campaign/lead"
            >캠페인</a
          >
          <div
            class="sub-menu rounded-b-lg hidden absolute w-[150px] left-0 bg-[#f05050] z-10"
          >
            <a
              class="sub-menu-item text-center no-underline text-lg py-3 bg-biz-red relative"
              href="/campaign/lead"
              >리드</a
            >
            <a
              class="sub-menu-item text-center no-underline text-lg py-3 bg-biz-red relative"
              href="/campaign/list"
              >리스트</a
            >
            <a
              class="sub-menu-item text-center no-underline text-lg py-3 bg-biz-red relative"
              href="/campaign/campaign"
              >캠페인</a
            >
          </div>
        </li>
        <li>
          <a
            class="nav-link px-0 relative flex items-center font-bold hover:text-biz-red text-[16px] text-center text-[#454545] h-[74px]"
            href="/plan/plan"
            >플랜</a
          >
        </li>
      </ul>
      <div
        class="hidden xl:flex items-center justify-end xl:ml-12 xl:mt-0 xl:justify-start"
      >
        <a
          href="/login/login"
          class="no-underline flex items-center text-black font-bold text-sm flex items-center mr-10"
          ><span class="login-icon mr-1"></span><span>로그인</span></a
        >
        <a
          href="/login/signupForm"
          class="no-underline flex items-center text-black font-bold text-sm flex items-center"
          ><span class="logout-icon mr-1"></span><span>회원가입</span></a
        >
      </div>
      <!-- 2 . 로그인 후 -->
      <!-- <div class="hidden xl:flex items-center justify-end xl:ml-12 xl:mt-0 xl:justify-start">
          <a href="../login/login.html" class="no-underline flex items-center text-black font-bold text-sm flex items-center mr-10"
            ><span class="login-icon mr-1"></span><span>로그아웃</span></a
          >
          <a href="../login/login.html" class="no-underline flex items-center text-black font-bold text-sm flex items-center"
            ><span class="logout-icon mr-1"></span><span>김호진님</span></a
          >
        </div> -->
    </nav>
    <!-- MOBILE 네비게이션 -->
    <div class="navbar-menu relative z-50" v-if="showButton">
      <div class="navbar-backdrop fixed inset-0 bg-gray-800 opacity-25"></div>
      <nav
        class="fixed top-0 left-0 bottom-0 flex flex-col w-5/6 max-w-sm py-3 px-6 bg-white border-r overflow-y-auto"
      >
        <div class="flex items-center mb-8">
          <a class="p-0 mr-auto" href="/main/main">
            <div class="logo"></div>
          </a>
          <button class="navbar-close">
            <svg
              class="h-6 w-6 text-gray-400 cursor-pointer hover:text-gray-500"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
              @click="toggleButton"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M6 18L18 6M6 6l12 12"
              ></path>
            </svg>
          </button>
        </div>
        <div>
          <ul>
            <li class="mb-1">
              <a
                class="nav-link py-2 h-full relative flex items-center font-bold text-md text-center text-[#454545]"
                href="/main/main"
                >HOME</a
              >
            </li>
            <li class="mb-1">
              <a
                class="nav-link py-2 h-full relative flex items-center font-bold text-md text-center text-[#454545]"
                href="#"
                >서비스 소개</a
              >
            </li>
            <li class="mb-1">
              <a
                class="nav-link py-2 h-full relative flex items-center font-bold text-md text-center text-[#454545]"
                href="#"
                >고객지원</a
              >
            </li>
            <li class="mb-1">
              <a
                class="nav-link py-2 h-full relative flex items-center font-bold text-md text-center text-[#454545]"
                href="/data/dataManagement"
                >데이터 관리</a
              >
            </li>
            <li class="mb-1">
              <details>
                <summary
                  class="nav-link py-2 w-full h-full relative flex items-center font-bold text-md text-center text-[#454545]"
                  href="/campaign/lead"
                >
                  캠페인
                  <svg
                    data-accordion-icon
                    class="w-6 h-6 shrink-0 ml-auto"
                    fill="currentColor"
                    viewBox="0 0 20 20"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                      clip-rule="evenodd"
                    ></path>
                  </svg>
                </summary>
                <div class="sub-menu rounded-b-lg block">
                  <a
                    class="sub-menu-item text-center no-underline text-md py-2 text-black lg:py-3"
                    href="/campaign/lead"
                    >리드</a
                  >
                  <a
                    class="sub-menu-item text-center no-underline text-md py-2 text-black lg:py-3"
                    href="/campaign/list"
                    >리스트</a
                  >
                  <a
                    class="sub-menu-item text-center no-underline text-md py-2 text-black lg:py-3"
                    href="/campaign/campaign"
                    >캠페인</a
                  >
                </div>
              </details>
            </li>
            <li class="mb-1">
              <a
                class="nav-link py-2 h-full relative flex items-center font-bold text-md text-center text-[#454545]"
                href="/plan/plan"
                >플랜</a
              >
            </li>
          </ul>
        </div>
        <div class="mt-auto">
          <div class="flex justify-end">
            <a
              href="/login/login"
              class="no-underline flex items-center text-black font-bold text-md flex items-center mr-4"
              ><span class="login-icon mr-1"></span><span>로그인</span></a
            >
            <a
              href="/login/signup"
              class="no-underline flex items-center text-black font-bold text-md flex items-center"
              ><span class="logout-icon mr-1"></span><span>회원가입</span></a
            >
          </div>
          <!-- 2 . 로그인 후 -->
          <!-- <div class="flex justify-end">
              <a href="../login/login.html" class="no-underline flex items-center text-black font-bold text-sm flex items-center mr-4"
                ><span class="login-icon mr-1"></span><span>로그아웃</span></a
              >
              <a href="../login/login.html" class="no-underline flex items-center text-black font-bold text-sm flex items-center"
                ><span class="logout-icon mr-1"></span><span>김호진님</span></a
              >
            </div> -->
        </div>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  data() {
    return {
      showButton: false,
    };
  },
  methods: {
    toggleButton() {
      this.showButton = !this.showButton;
      console.log(this.showButton);
    },
  },
};
</script>
