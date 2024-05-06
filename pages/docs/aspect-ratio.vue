<template>
<div>
  <div class="preview flex min-h-[50px] w-full justify-center p-10 items-center">
    <a href="https://www.shadcn-vue.com/docs/components/aspect-ratio.html"  target="_blank">shadcn-vue docs</a>
  </div>
  <div class="preview flex min-h-[50px] max-w-[600px] justify-center p-10 items-center">
    <!-- 这里填写组件 -->
    <UiAspectRatio :ratio="16/9" class="bg-muted">
    <img
      src="https://images.unsplash.com/photo-1588345921523-c2dcdb7f1dcd?w=800&dpr=2&q=80"
      alt="Photo by Drew Beamer"
      class="rounded-md object-cover w-full h-full"
    >
  </UiAspectRatio>
    <!-- 这里填写组件 -->
  </div>
</div>
</template>

<script lang="ts" setup>

</script>

<style>

</style>