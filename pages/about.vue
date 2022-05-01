<template>
  <div>
    <div class="carousel relative container mx-auto">
      <div class="carousel-inner relative overflow-hidden w-full">
        <input class="carousel-open" type="radio" id="carousel-1" name="carousel" aria-hidden="true" hidden="" checked="checked">
        <div class="carousel-item absolute opacity-0" style="height:50vh;">
          <div class="slide-1 block h-full w-full mx-auto flex pt-6 md:pt-0 md:items-center bg-cover bg-right">
            <div class="container mx-auto">
              <div class="text-white text-4xl cursor-pointer absolute bottom-8 w-full lg:w-1/2 md:ml-16 items-center md:items-start px-6 tracking-wide">
                {{ $t('about') }}
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="container mx-auto">

    </div>
  </div>
</template>

<script>
export default {
  name: "about"
}
</script>

<style scoped>
.slide-1{
  background: url('../images/lion.jpeg') center -125px;
}
@media only screen and (min-width: 1440px) {
  .carousel{
    max-width:1600px;
  }
}
</style>
