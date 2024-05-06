<template>
<div>
  <div class="preview flex min-h-[50px] w-full justify-center p-10 items-center">
    <a href="https://www.shadcn-vue.com/docs/components/avatar.html"  target="_blank" class="text-blue-500 hover:underline">component docs</a>
    <div class="w-8"/>
    <a href="https://www.radix-vue.com/components/avatar.html"  target="_blank" class="text-blue-500 hover:underline">api docs</a>
  </div>
  <div class="preview flex min-h-[50px] w-auto justify-center p-10 items-center space-x-4 bg-gray-100 rounded-lg mx-10">
    <!-- 这里填写组件 -->
    <UiAvatar>
        <UiAvatarImage
      src="https://images.unsplash.com/photo-1492633423870-43d1cd2775eb?&w=128&h=128&dpr=2&q=80"
      alt="Colm Tuite"
      fallback="CT"
      :delay-ms="600"
    /> 
    </UiAvatar>
    <UiAvatar>
        <UiAvatarImage
            src="https://images.unsplash.com/photo-1511485977113-f34c92461ad9?ixlib=rb-1.2.1&w=128&h=128&dpr=2&q=80"
            alt="Colm Tuite"
            fallback='ct'
            :delay-ms="600"
    /> 
        <UiAvatarFallback :delay-ms="600" >JD</UiAvatarFallback>
    </UiAvatar>
    <UiAvatar>
    <UiAvatarFallback>JD</UiAvatarFallback>
    </UiAvatar>
    <!-- 这里填写组件 -->
  </div>
</div>
</template>

<script lang="ts" setup>

</script>

<style>

</style>