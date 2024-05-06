<template>
<div>
  <div class="preview flex min-h-[50px] w-full justify-center p-10 items-center">
    <a href="https://www.shadcn-vue.com/docs/components/label"  target="_blank" class="text-blue-500 hover:underline">component docs</a>
    <div class="w-8"/>
    <a href="https://www.radix-vue.com/components/label"  target="_blank" class="text-blue-500 hover:underline">api docs</a>
  </div>
  <div class="preview flex min-h-[50px] w-auto justify-center p-10 items-center space-x-4 bg-gray-100 rounded-lg mx-10">
    <!-- 这里填写组件 -->
    <div class="flex items-center space-x-2">
      <UiCheckbox id="terms" />
      <UiLabel for="terms">Accept terms and conditions</UiLabel>
    </div>
    <!-- 这里填写组件 -->
  </div>
</div>
</template>

<script lang="ts" setup>

</script>

<style>

</style>