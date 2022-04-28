<template>
  <div>
    <footer class="p-4 bg-white rounded-lg shadow md:px-6 md:py-8 dark:bg-gray-800">
      <div class="flex justify-between items-center">
        <nuxt-link :to="localePath('/')" class="flex items-center">
          <img data-v-1a9bb128="" src="https://img.icons8.com/ios/50/000000/museum.png">
          <span class="flex items-center tracking-wide no-underline hover:no-underline font-bold text-gray-800 text-xl ">CILICIA</span>
        </nuxt-link>
        <div>
          <p class="text-sm text-gray-500 sm:text-center dark:text-gray-400">Tel: +374 99-308-708</p>
          <p class="text-sm text-gray-500 sm:text-center dark:text-gray-400">Email: cilicia@museum.com</p>
        </div>
      </div>
      <div class="sm:flex sm:items-center sm:justify-between">
        <ul class="flex flex-wrap items-center mb-6 text-sm text-gray-500 sm:mb-0 dark:text-gray-400">
          <li>
            <nuxt-link :to="localePath('/')" class="mr-4 hover:underline md:mr-6">{{ $t('home') }}</nuxt-link>
          </li>
          <li>
            <nuxt-link :to="localePath('/')" class="mr-4 hover:underline md:mr-6">{{ $t('history') }}</nuxt-link>
          </li>
          <li>
            <nuxt-link :to="localePath('/')" class="mr-4 hover:underline md:mr-6">{{ $t('gallery') }}</nuxt-link>
          </li>
          <li>
            <nuxt-link :to="localePath('/')" class="mr-4 hover:underline md:mr-6">{{ $t('event') }}</nuxt-link>
          </li>
        </ul>
      </div>
      <hr class="my-6 border-gray-200 sm:mx-auto dark:border-gray-700 lg:my-8">
      <span class="block text-sm text-gray-500 sm:text-center dark:text-gray-400">© 2022 <span class="hover:underline">Cilicia museum</span>. All Rights Reserved.
      </span>
    </footer>
  </div>
</template>

<script>
  export default {
    name: "Footer"
  }
</script>

<style scoped>

</style>
