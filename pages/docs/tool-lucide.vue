<template>
<div>
  <div class="preview flex min-h-[50px] w-full justify-center p-10 items-center">
    <a href="https://lucide.dev/icons/calendar-days"  target="_blank" class="text-blue-500 hover:underline">lucide icon docs</a>
    <div class="w-8"/>
    <a href="https://lucide.dev/guide/packages/lucide-vue-next"  target="_blank" class="text-blue-500 hover:underline">lucide vue docs</a>
  </div>
  <div class="preview flex min-h-[50px] w-auto justify-center p-10 items-center space-x-4 bg-gray-100 rounded-lg mx-10">
    <!-- fill component -->
       <Brush color="#3e9392" size=18 /> <a href="https://lucide.dev/icons/"  target="_blank" class="text-blue-500 hover:underline">Lucide Icons</a>
    <!-- fill component -->
  </div>


</div>
</template>

<script lang="ts" setup>
import { Brush } from 'lucide-vue-next';
</script>

<style>

</style>