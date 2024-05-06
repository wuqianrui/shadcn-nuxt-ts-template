<template>
<div>
  <div class="preview flex min-h-[50px] w-full justify-center p-10 items-center">
    <a href="https://www.shadcn-vue.com/docs/components/separator"  target="_blank" class="text-blue-500 hover:underline">component docs</a>
    <div class="w-8"/>
    <a href="https://www.radix-vue.com/components/separator"  target="_blank" class="text-blue-500 hover:underline">api docs</a>
  </div>
  <div class="preview flex min-h-[50px] w-auto justify-center p-10 items-center space-x-4 bg-gray-100 rounded-lg mx-10">
    <!-- fill component -->
    <div>
      <div class="space-y-1">
      <h4 class="text-sm font-medium leading-none">
        Radix Primitives
      </h4>
      <p class="text-sm text-muted-foreground">
        An open-source UI component library.
      </p>
    </div>
    <UiSeparator class="my-4" />
    <div class="flex h-5 items-center space-x-4 text-sm">
      <div>Blog</div>
      <UiSeparator orientation="vertical" decorative/>
      <div>Docs</div>
      <UiSeparator orientation="vertical" />
      <div>Source</div>
    </div>
    <UiSeparator class="my-4" decorative />
    </div>
    <!-- fill component -->
  </div>
</div>
</template>

<script lang="ts" setup>

</script>

<style>

</style>