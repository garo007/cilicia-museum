<template>
  <div>
    <SlideShow/>
    <div class="container mx-auto">
      <h3 class="font-medium leading-tight text-3xl mt-10 mb-2 text-center">{{$t('gallery')}}</h3>
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
    </div>
    <div class="container mx-auto">
      <h3 class="font-medium leading-tight text-3xl mt-10 mb-2 text-center">{{$t('event')}}</h3>
      <div class="grid-cols-2 px-20 py-6 space-y-2 lg:space-y-0 lg:grid lg:gap-2">
        <div class="w-11/12 rounded">
          <div>
            <img src="../images/castle3.jpg"
                 alt="image" style="max-width: 370px">
          </div>
          <div>
            <h1 class="flex-auto text-lg font-semibold text-slate-900">
              {{$t('events.building.title')}}
            </h1>
            <p class="text-sm text-slate-700 date">{{$t('events.building.date')}}</p>
          </div>
        </div>
        <div class="w-11/12 rounded">
          <div>
            <img src="../images/coin.jpg"
                 alt="image"  style="max-width: 370px">
          </div>
          <div>
            <h1 class="flex-auto text-lg font-semibold text-slate-900">
              {{$t('events.coin.title')}}
            </h1>
            <p class="text-sm text-slate-700 date">{{$t('events.coin.date')}}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'IndexPage'
}
</script>

<style>
  .date{
    background: linear-gradient(to right, rgba(241, 145, 0, 0.8) 0%, rgba(199, 64, 64, 0.8) 100%);
    color: #fff;
    text-align: center;
    padding: 5px 25px;
    border-radius: 10px;
    width: fit-content;
  }
</style>
