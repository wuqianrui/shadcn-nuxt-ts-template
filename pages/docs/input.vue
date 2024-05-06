<template>
<div>
  <div class="preview flex min-h-[50px] w-full justify-center p-10 items-center">
    <a href="https://www.shadcn-vue.com/docs/components/input"  target="_blank" class="text-blue-500 hover:underline">component docs</a>
    <div class="w-8"/>
    <a href=""  target="_blank" class="text-blue-500 hover:underline">api docs</a>
  </div>
  <div class="preview flex min-h-[50px] w-auto justify-center p-10 items-center space-x-4 bg-gray-100 rounded-lg mx-10">
    <!-- component 01 -->
    <div class="grid w-full max-w-sm items-center gap-1.5">
      <UiLabel for="search">Icon Input</UiLabel>
      <div class="relative w-full max-w-sm items-center">
      <UiInput id="search" type="text" placeholder="Search..." class="pl-10" />
      <span class="absolute start-0 inset-y-0 flex items-center justify-center px-2">
        <Search class="size-6 text-muted-foreground" />
      </span>
    </div>
  </div>
    <!-- component 01 -->
  </div>
  <!-- component 02 -->
    <div class="preview flex min-h-[50px] w-auto justify-center p-10 items-center space-x-4 bg-gray-100 rounded-lg mx-10">
      <div class="grid w-full max-w-sm items-center gap-1.5">
      <UiLabel for="picture">Picture</UiLabel>
      <UiInput id="picture" type="file" />
      </div>
    </div>
    <!-- component 02 -->
    <!-- component 03 -->
    <div class="preview flex min-h-[50px] w-auto justify-center p-10 items-center space-x-4 bg-gray-100 rounded-lg mx-10">

    <div class="grid w-full max-w-sm items-center gap-1.5">
      <UiLabel for="email">Email</UiLabel>
      <UiInput id="email" type="email" placeholder="Email" />
    </div>
    </div>
    <!-- component 03 -->

</div>
</template>

<script lang="ts" setup>
import { Search } from 'lucide-vue-next'
</script>

<style>

</style>