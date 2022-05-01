<template>
  <div>
    <div class="carousel relative container mx-auto">
      <div class="carousel-inner relative overflow-hidden w-full">
        <input class="carousel-open" type="radio" id="carousel-1" name="carousel" aria-hidden="true" hidden=""
               checked="checked">
        <div class="carousel-item absolute opacity-0" style="height:50vh;">
          <div class="slide-1 block h-full w-full mx-auto flex pt-6 md:pt-0 md:items-center bg-cover bg-right">
            <div class="container mx-auto">
              <div
                class="about-history text-white cursor-pointer w-full lg:w-1/2 md:ml-16 items-center md:items-start px-6 tracking-wide">
                {{ $t('gallery') }}
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="container mx-auto">
      <h3 class="font-medium leading-tight text-3xl mt-10 mb-2 text-center">{{ $t('gallery') }}</h3>
      <div class="grid-cols-3 px-20 py-6 space-y-2 lg:space-y-0 lg:grid lg:gap-3">
        <div class="w-full rounded">
          <img src="../images/tur.jpg"
               alt="image">
        </div>
        <div class="w-full rounded">
          <img src="../images/qandak.jpg"
               alt="image">
        </div>
        <div class="w-full rounded">
          <img src="../images/kuj.jpg"
               alt="image">
        </div>
      </div>
      <div class="grid-cols-3 px-20 py-6 space-y-2 lg:space-y-0 lg:grid lg:gap-3">
        <div class="w-full rounded">
          <img src="../images/coin.jpg"
               alt="image">
        </div>
        <div class="w-full rounded">
          <img src="../images/armpor.jpg"
               alt="image">
        </div>
        <div class="w-full rounded">
          <img src="../images/coin2.jpg"
               alt="image">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "about"
}
</script>

<style scoped>
.slide-1 {
  background-image: url('../images/baner.jpeg');
}

@media only screen and (min-width: 1440px) {
  .carousel {
    max-width: 1600px;
  }

  .about-history {
    text-transform: uppercase;
    opacity: 0.7;
    text-align: center;
    font-size: 9vw;
  }
}
</style>
