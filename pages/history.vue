<template>
  <div>
    <div class="carousel relative container mx-auto">
      <div class="carousel-inner relative overflow-hidden w-full">
        <input class="carousel-open" type="radio" id="carousel-1" name="carousel" aria-hidden="true" hidden="" checked="checked">
        <div class="carousel-item absolute opacity-0" style="height:50vh;">
          <div class="slide-1 block h-full w-full mx-auto flex pt-6 md:pt-0 md:items-center bg-cover bg-right">
            <div class="container mx-auto">
              <div class="about-history text-white cursor-pointer w-full lg:w-1/2 md:ml-16 items-center md:items-start px-6 tracking-wide">
                {{ $t('history') }}
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
      <div class="container mx-auto about-lion">
        <h3 class="font-medium leading-tight text-3xl mt-10 mb-2 font-medium text-center uppercase">{{$t('history')}}</h3>
        <div class="mx-auto w-1/2 text-justify">
          <p class="mt-3">{{$t('about_history_part_1')}}</p>
          <p class="mt-3">{{$t('about_history_part_2')}} </p>
          <p class="mt-3">{{$t('about_history_part_3')}}</p>
          <p class="mt-3">{{$t('about_history_part_4')}}</p>
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
  background-image: url('../images/map.jpeg');
}
.about-lion {
  background: url('../images/lion-removebg-preview-removebg-preview.png') no-repeat center;
  background-size: contain;
}
@media only screen and (min-width: 1440px) {
  .carousel{
    max-width:1600px;
  }
  .about-history{
    text-transform: uppercase;
    opacity: 0.7;
    text-align: center;
    font-size: 9vw;
  }
}
</style>
