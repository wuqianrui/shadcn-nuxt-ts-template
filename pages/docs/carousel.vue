<template>
<div>
  <div class="preview flex min-h-[50px] w-full justify-center p-10 items-center">
    <a href="https://www.shadcn-vue.com/docs/components/carousel"  target="_blank" class="text-blue-500 hover:underline">component docs</a>
    <div class="w-8"/>
    <a href="https://www.embla-carousel.com/api"  target="_blank" class="text-blue-500 hover:underline">api docs</a>
  </div>
  <div class="preview flex min-h-[50px] w-auto justify-center p-10 items-center space-x-4 bg-gray-100 rounded-lg mx-10">
    <!-- fill component -->
    <UiCarousel class="relative w-full max-w-xs">
    <UiCarouselContent>
      <UiCarouselItem v-for="(imgItem, index) in imgUrls" :key="index" >
        <div class="p-1 img-card h-full flex justify-center items-center" @click="previewImg(index)">
          <img :src="imgItem.src" />
        </div>
      </UiCarouselItem>
    </UiCarouselContent>
    <UiCarouselPrevious />
    <UiCarouselNext />
  </UiCarousel>
    <!-- fill component -->
  </div>
  <div  class="preview flex w-auto justify-center p-10 items-center mx-10">
    use <a href="https://github.com/hzpeng57/vue-preview-imgs" target="_blank" class="text-blue-500 mx-2">vue-preview-imgs</a> package , image 's preview api .
  </div>
</div>
</template>

<script lang="ts" setup>
import { setGallery } from "vue-preview-imgs";

const imgUrls = [{
    src: 'https://images.unsplash.com/photo-1492633423870-43d1cd2775eb?&w=128&h=128&dpr=2&q=80',
    msrc: 'xxx',
    alt: 'picture2',
    w: 1024,
    h: 683,
  },
  {
    src: 'https://farm4.staticflickr.com/3902/14985871946_86abb8c56f_b.jpg',
    msrc: 'xxx',
    alt: 'picture2',
    w: 1024,
    h: 683,
  }
  ,{
    src: 'https://github.com/waynecz/vue-img-inputer/raw/master/src/assets/vip-logo.png',
    msrc: 'xxx',
    w: 1024,
    h: 683,
  }]

  function previewImg(index:number){
    const lightbox = setGallery({
      dataSource: imgUrls,
    });

    lightbox.loadAndOpen(index);
  }
</script>

<style>

.img{
  border-radius: 1.8rem;
  display: block;
  height: 19rem;
  width: 100%;
  object-fit: cover;
}
</style>