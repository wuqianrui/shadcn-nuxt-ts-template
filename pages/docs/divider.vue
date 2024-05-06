<template>
<div>
  <div class="preview flex min-h-[50px] w-full justify-center p-10 items-center">
    <a href="$web_url$"  target="_blank" class="text-blue-500 hover:underline">component docs</a>
    <div class="w-8"/>
    <a href=""  target="_blank" class="text-blue-500 hover:underline">api docs</a>
  </div>
  <div class="preview flex-col min-h-[50px] w-auto justify-center p-10 items-center space-x-4 bg-gray-100 rounded-lg mx-10">
    <!-- fill component -->
    <div class="flex w-full items-center">
    <UiDivider label="OR" />
    </div>
    <!-- fill component -->
  </div>

  <div class="h-5"></div>

  <div class="preview flex-col min-h-[50px] w-auto justify-center p-10 items-center space-x-4 bg-gray-100 rounded-lg mx-10">
    <!-- fill component -->
    <div class="flex w-full items-center">
    <UiDivider icon="lucide:activity" />
    </div>
    <!-- fill component -->
  </div>

  <div class="h-5"></div>

  <div class="preview w-auto justify-center p-10 rounded-lg ">
    <!-- fill component -->
    <div class="flex h-[200px] w-full items-center">
    <UiDivider orientation="vertical" avatar="https://avatars.githubusercontent.com/u/66577?s=80&v=4" />
    </div>
    <!-- fill component -->
  </div>

  
    
</div>
</template>

<script lang="ts" setup>

</script>

<style>

</style>