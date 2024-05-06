<template>
<div>
  <div class="preview flex min-h-[50px] w-full justify-center p-10 items-center">
    <a href="https://www.shadcn-vue.com/docs/components/button"  target="_blank" class="text-blue-500 hover:underline">component docs</a>
  </div>
  <div class="preview flex min-h-[50px] w-auto justify-center p-10 items-center space-x-4 bg-gray-100 rounded-lg mx-10">
    <!-- 这里填写组件 -->
    <UiButton>Default</UiButton>
      <UiButton variant="secondary">Secondary</UiButton>
      <UiButton><Icon class="h-4 w-4 mr-2" name="lucide:mail" /> Login with Email</UiButton>
      <UiButton loading
        ><Icon class="h-4 w-4 animate-spin mr-2" name="lucide:loader-2" /> Please wait</UiButton
      >
      <UiButton variant="outline">Outline</UiButton>
      <UiButton variant="destructive">Destructive</UiButton>
      <UiButton variant="ghost">Ghost</UiButton>
      <UiButton variant="link">Link Btn</UiButton>
      <UiButton variant="outline" size="icon"
        ><Icon class="h-4 w-4" name="lucide:activity"
      /></UiButton>

      <UiChip variant="success" position="bottom-right" size="md" text="3">
        <UiButton variant="outline" size="icon"
        ><Icon class="h-4 w-4" name="lucide:activity"
      /></UiButton>
      </UiChip>
    <!-- 这里填写组件 -->
  </div>
</div>
</template>

<script lang="ts" setup>

</script>

<style>

</style>