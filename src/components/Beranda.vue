<template>
  
  <div>
    <nav class="bg-gray-800">
  <div class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8">
    <div class="relative flex h-16 items-center justify-between">
      <div class="absolute inset-y-0 left-0 flex items-center sm:hidden">
        <!-- Mobile menu button-->
        <button type="button" class="relative inline-flex items-center justify-center rounded-md p-2 text-gray-400 hover:bg-gray-700 hover:text-white focus:outline-none focus:ring-2 focus:ring-inset focus:ring-white" aria-controls="mobile-menu" aria-expanded="false">
          <span class="absolute -inset-0.5"></span>
          <span class="sr-only">Open main menu</span>
          <!--
            Icon when menu is closed.

            Menu open: "hidden", Menu closed: "block"
          -->
          <svg class="block h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true">
            <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
          </svg>
          <!--
            Icon when menu is open.

            Menu open: "block", Menu closed: "hidden"
          -->
          <svg class="hidden h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true">
            <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
          </svg>
        </button>
      </div>
      <div class="flex flex-1 items-center justify-center sm:items-stretch sm:justify-start">
        <div class="flex flex-shrink-0 items-center">
          <img class="h-8 w-auto" src="https://tailwindui.com/img/logos/mark.svg?color=indigo&shade=500" alt="Your Company">
        </div>
        <div class="hidden sm:ml-6 sm:block">
          <div class="flex space-x-4">
            <!-- Current: "bg-gray-900 text-white", Default: "text-gray-300 hover:bg-gray-700 hover:text-white" -->
            <a href="#" class="bg-gray-900 text-white rounded-md px-3 py-2 text-sm font-medium" aria-current="page">Home</a>
            <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white rounded-md px-3 py-2 text-sm font-medium">about</a>
            <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white rounded-md px-3 py-2 text-sm font-medium">contact</a>
          </div>
        </div>
      </div>
      <div class="absolute inset-y-0 right-0 flex items-center pr-2 sm:static sm:inset-auto sm:ml-6 sm:pr-0">
        <button type="button" class="relative rounded-full bg-gray-800 p-1 text-gray-400 hover:text-white focus:outline-none focus:ring-2 focus:ring-white focus:ring-offset-2 focus:ring-offset-gray-800">
          <span class="absolute -inset-1.5"></span>
          <span class="sr-only">View notifications</span>
          <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true">
            <path stroke-linecap="round" stroke-linejoin="round" d="M14.857 17.082a23.848 23.848 0 005.454-1.31A8.967 8.967 0 0118 9.75v-.7V9A6 6 0 006 9v.75a8.967 8.967 0 01-2.312 6.022c1.733.64 3.56 1.085 5.455 1.31m5.714 0a24.255 24.255 0 01-5.714 0m5.714 0a3 3 0 11-5.714 0" />
          </svg>
        </button>

        <!-- Profile dropdown -->
        <div class="relative ml-3">
          <div>
            <button type="button" class="relative flex rounded-full bg-gray-800 text-sm focus:outline-none focus:ring-2 focus:ring-white focus:ring-offset-2 focus:ring-offset-gray-800" id="user-menu-button" aria-expanded="false" aria-haspopup="true">
              <span class="absolute -inset-1.5"></span>
              <span class="sr-only">Open user menu</span>
              <img class="h-8 w-8 rounded-full" src="../assets/profil.jpeg" alt="">
            </button>
          </div>

          <!--
            Dropdown menu, show/hide based on menu state.

            Entering: "transition ease-out duration-100"
              From: "transform opacity-0 scale-95"
              To: "transform opacity-100 scale-100"
            Leaving: "transition ease-in duration-75"
              From: "transform opacity-100 scale-100"
              To: "transform opacity-0 scale-95"
          -->
      
        </div>
      </div>
    </div>
  </div>

  <!-- Mobile menu, show/hide based on menu state. -->
  <div class="sm:hidden" id="mobile-menu">
    <div class="space-y-1 px-2 pb-3 pt-2">
      <!-- Current: "bg-gray-900 text-white", Default: "text-gray-300 hover:bg-gray-700 hover:text-white" -->
      <a href="#" class="bg-gray-900 text-white block rounded-md px-3 py-2 text-base font-medium" aria-current="page">Dashboard</a>
      <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md px-3 py-2 text-base font-medium">Team</a>
      <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md px-3 py-2 text-base font-medium">Projects</a>
      <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md px-3 py-2 text-base font-medium">Calendar</a>
    </div>
  </div>
</nav>
  </div>
  <svg id="wave" style="transform:rotate(180deg); transition: 0.3s" viewBox="0 0 1440 390" version="1.1" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="sw-gradient-0" x1="0" x2="0" y1="1" y2="0"><stop stop-color="rgba(237.52, 2.249, 255, 1)" offset="0%"></stop><stop stop-color="rgba(233.641, 14.411, 241.659, 1)" offset="100%"></stop></linearGradient></defs><path style="transform:translate(0, 0px); opacity:1" fill="url(#sw-gradient-0)" d="M0,234L15,253.5C30,273,60,312,90,318.5C120,325,150,299,180,266.5C210,234,240,195,270,208C300,221,330,286,360,305.5C390,325,420,299,450,266.5C480,234,510,195,540,156C570,117,600,78,630,91C660,104,690,169,720,169C750,169,780,104,810,97.5C840,91,870,143,900,169C930,195,960,195,990,201.5C1020,208,1050,221,1080,240.5C1110,260,1140,286,1170,286C1200,286,1230,260,1260,247C1290,234,1320,234,1350,234C1380,234,1410,234,1440,221C1470,208,1500,182,1530,195C1560,208,1590,260,1620,247C1650,234,1680,156,1710,130C1740,104,1770,130,1800,156C1830,182,1860,208,1890,234C1920,260,1950,286,1980,266.5C2010,247,2040,182,2070,182C2100,182,2130,247,2145,279.5L2160,312L2160,390L2145,390C2130,390,2100,390,2070,390C2040,390,2010,390,1980,390C1950,390,1920,390,1890,390C1860,390,1830,390,1800,390C1770,390,1740,390,1710,390C1680,390,1650,390,1620,390C1590,390,1560,390,1530,390C1500,390,1470,390,1440,390C1410,390,1380,390,1350,390C1320,390,1290,390,1260,390C1230,390,1200,390,1170,390C1140,390,1110,390,1080,390C1050,390,1020,390,990,390C960,390,930,390,900,390C870,390,840,390,810,390C780,390,750,390,720,390C690,390,660,390,630,390C600,390,570,390,540,390C510,390,480,390,450,390C420,390,390,390,360,390C330,390,300,390,270,390C240,390,210,390,180,390C150,390,120,390,90,390C60,390,30,390,15,390L0,390Z"></path><defs><linearGradient id="sw-gradient-1" x1="0" x2="0" y1="1" y2="0"><stop stop-color="rgba(243.936, 22.81, 199.305, 1)" offset="0%"></stop><stop stop-color="rgba(196.124, 42.699, 102.791, 1)" offset="100%"></stop></linearGradient></defs><path style="transform:translate(0, 50px); opacity:0.9" fill="url(#sw-gradient-1)" d="M0,195L15,221C30,247,60,299,90,312C120,325,150,299,180,299C210,299,240,325,270,292.5C300,260,330,169,360,156C390,143,420,208,450,227.5C480,247,510,221,540,221C570,221,600,247,630,240.5C660,234,690,195,720,162.5C750,130,780,104,810,136.5C840,169,870,260,900,286C930,312,960,273,990,273C1020,273,1050,312,1080,292.5C1110,273,1140,195,1170,188.5C1200,182,1230,247,1260,227.5C1290,208,1320,104,1350,91C1380,78,1410,156,1440,156C1470,156,1500,78,1530,58.5C1560,39,1590,78,1620,110.5C1650,143,1680,169,1710,182C1740,195,1770,195,1800,175.5C1830,156,1860,117,1890,97.5C1920,78,1950,78,1980,97.5C2010,117,2040,156,2070,175.5C2100,195,2130,195,2145,195L2160,195L2160,390L2145,390C2130,390,2100,390,2070,390C2040,390,2010,390,1980,390C1950,390,1920,390,1890,390C1860,390,1830,390,1800,390C1770,390,1740,390,1710,390C1680,390,1650,390,1620,390C1590,390,1560,390,1530,390C1500,390,1470,390,1440,390C1410,390,1380,390,1350,390C1320,390,1290,390,1260,390C1230,390,1200,390,1170,390C1140,390,1110,390,1080,390C1050,390,1020,390,990,390C960,390,930,390,900,390C870,390,840,390,810,390C780,390,750,390,720,390C690,390,660,390,630,390C600,390,570,390,540,390C510,390,480,390,450,390C420,390,390,390,360,390C330,390,300,390,270,390C240,390,210,390,180,390C150,390,120,390,90,390C60,390,30,390,15,390L0,390Z"></path><defs><linearGradient id="sw-gradient-2" x1="0" x2="0" y1="1" y2="0"><stop stop-color="rgba(33.922, 195.089, 255, 1)" offset="0%"></stop><stop stop-color="rgba(255, 13.767, 165.453, 1)" offset="100%"></stop></linearGradient></defs><path style="transform:translate(0, 100px); opacity:0.8" fill="url(#sw-gradient-2)" d="M0,0L15,13C30,26,60,52,90,84.5C120,117,150,156,180,149.5C210,143,240,91,270,91C300,91,330,143,360,169C390,195,420,195,450,201.5C480,208,510,221,540,214.5C570,208,600,182,630,149.5C660,117,690,78,720,91C750,104,780,169,810,221C840,273,870,312,900,318.5C930,325,960,299,990,273C1020,247,1050,221,1080,214.5C1110,208,1140,221,1170,234C1200,247,1230,260,1260,279.5C1290,299,1320,325,1350,299C1380,273,1410,195,1440,162.5C1470,130,1500,143,1530,182C1560,221,1590,286,1620,260C1650,234,1680,117,1710,78C1740,39,1770,78,1800,78C1830,78,1860,39,1890,26C1920,13,1950,26,1980,65C2010,104,2040,169,2070,208C2100,247,2130,260,2145,266.5L2160,273L2160,390L2145,390C2130,390,2100,390,2070,390C2040,390,2010,390,1980,390C1950,390,1920,390,1890,390C1860,390,1830,390,1800,390C1770,390,1740,390,1710,390C1680,390,1650,390,1620,390C1590,390,1560,390,1530,390C1500,390,1470,390,1440,390C1410,390,1380,390,1350,390C1320,390,1290,390,1260,390C1230,390,1200,390,1170,390C1140,390,1110,390,1080,390C1050,390,1020,390,990,390C960,390,930,390,900,390C870,390,840,390,810,390C780,390,750,390,720,390C690,390,660,390,630,390C600,390,570,390,540,390C510,390,480,390,450,390C420,390,390,390,360,390C330,390,300,390,270,390C240,390,210,390,180,390C150,390,120,390,90,390C60,390,30,390,15,390L0,390Z"></path></svg>
</template>