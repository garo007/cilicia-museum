<template>
  <div>
<!--  <nav class="flex items-center justify-between flex-wrap bg-teal">-->
<!--    <div class="flex items-center flex-no-shrink text-white mr-6 logo">-->
<!--      <div class="logo-wrap">-->
<!--        <nuxt-link :to="localePath('/')">-->
<!--          <div class="logo-and-name">-->
<!--            <div class="mx-5" style='background-image: url()'>-->
<!--              <img src="" alt="">-->
<!--            </div>-->
<!--            <div class="mx-8">-->
<!--              <h4 class="font-semibold text-xl text-slate-600 cilicia_text">Cilicia</h4>-->
<!--              <p class="text-amber-400 cilicia_text_slogan">History Museum</p>-->
<!--            </div>-->
<!--          </div>-->
<!--        </nuxt-link>-->
<!--      </div>-->
<!--    </div>-->
<!--    <div class="block lg:hidden">-->
<!--      <button class="flex items-center px-3 py-2 border rounded text-teal-lighter border-teal-light hover:text-white hover:border-white">-->
<!--        <svg class="h-3 w-3" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><title>Menu</title><path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"/></svg>-->
<!--      </button>-->
<!--    </div>-->
<!--  </nav>-->
  <nav id="header" class="w-full z-30 top-0 py-1">
    <div class="w-full container mx-auto flex flex-wrap items-center justify-between mt-0 px-6 py-3">

      <label for="menu-toggle" class="cursor-pointer md:hidden block">
        <svg class="fill-current text-gray-900" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 20 20">
          <title>menu</title>
          <path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"></path>
        </svg>
      </label>
      <input class="hidden" type="checkbox" id="menu-toggle">

      <div class="hidden md:flex md:items-center md:w-auto w-full order-3 md:order-1" id="menu">
        <nav>
          <ul class="md:flex items-center justify-between text-base text-gray-700 pt-4 md:pt-0">
            <li><nuxt-link class="inline-block no-underline hover:text-black hover:underline py-2 px-4" :to="localePath('/')">{{ $t('home') }}</nuxt-link></li>
            <li><nuxt-link class="inline-block no-underline hover:text-black hover:underline py-2 px-4" :to="localePath('/history')">{{ $t('history') }}</nuxt-link></li>
            <li><nuxt-link class="inline-block no-underline hover:text-black hover:underline py-2 px-4" :to="localePath('/gallery')">{{ $t('gallery') }}</nuxt-link></li>
            <li><nuxt-link class="inline-block no-underline hover:text-black hover:underline py-2 px-4" :to="localePath('/event')">{{ $t('event') }}</nuxt-link></li>
          </ul>
        </nav>
      </div>



      <div id="nav-content">
        <div class="order-1 md:order-2">
          <a class="flex items-center tracking-wide no-underline hover:no-underline font-bold text-gray-800 text-xl " href="#">
            <img src="https://img.icons8.com/ios/50/000000/museum.png"/>
            CILICIA
          </a>
        </div>
      </div>
      <div class="order-2 md:order-3 flex items-center">
        <LanguageInput/>
      </div>
    </div>
  </nav>
</div>
</template>

<script>
export default {
  name: "Header"
}
</script>

<style scoped>
  .logo-wrap img {
    height: 100px;
    width: 100%;
  }
</style>
