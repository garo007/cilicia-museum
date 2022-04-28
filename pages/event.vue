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
                class="about-history text-black cursor-pointer w-full lg:w-1/2 items-center md:items-start tracking-wide">
                {{ $t('event') }}
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="container mx-auto">
      <h3 class="font-medium leading-tight text-3xl mt-10 mb-2 text-center">{{ $t('event') }}</h3>
      <div class="grid-cols-2 px-20 py-6 space-y-2 lg:space-y-0 lg:grid lg:gap-2">
        <div class="w-11/12 rounded">
          <div>
            <img src="../images/castle3.jpg"
                 alt="image" style="max-width: 370px">
          </div>
          <div>
            <h1 class="flex-auto text-lg font-semibold text-slate-900">
              {{ $t('events.building.title') }}
            </h1>
            <p class="text-sm text-slate-700 date">{{ $t('events.building.date') }}</p>
          </div>
        </div>
        <div class="w-11/12 rounded">
          <div>
            <img src="../images/coin.jpg"
                 alt="image" style="max-width: 370px">
          </div>
          <div>
            <h1 class="flex-auto text-lg font-semibold text-slate-900">
              {{ $t('events.coin.title') }}
            </h1>
            <p class="text-sm text-slate-700 date">{{ $t('events.coin.date') }}</p>
          </div>
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
  background: url('../images/krish.jpeg') center -22px;;
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

.date {
  background: linear-gradient(to right, rgba(241, 145, 0, 0.8) 0%, rgba(199, 64, 64, 0.8) 100%);
  color: #fff;
  text-align: center;
  padding: 5px 25px;
  border-radius: 10px;
  width: fit-content;
}
.rounded img {
  height: 270px;
}
</style>
