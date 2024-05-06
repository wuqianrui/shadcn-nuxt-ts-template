<template>
<div>
  <div class="preview flex min-h-[50px] w-full justify-center p-10 items-center">
    <a href="https://ui-thing.behonbaker.com/components/badge#usage"  target="_blank">shadcn-vue docs</a>
  </div>
  <div class="preview flex min-h-[50px] w-full justify-center p-10 items-center">
    <!-- 这里填写组件 -->
    <div class="preview flex min-h-[50px] w-auto justify-center p-10 items-center space-x-4 bg-gray-100 rounded-lg mx-10">
        <UiBadge>Default</UiBadge>
    <UiBadge variant="destructive">Destructive</UiBadge>
    <UiBadge variant="outline">Outline</UiBadge>
    <UiBadge variant="secondary">Secondary</UiBadge>
    <UiBadge variant="success">success</UiBadge>
    <UiBadge variant="warning">warning</UiBadge>
    <UiBadge variant="danger">danger</UiBadge>

    </div>
    <!-- 这里填写组件 -->
  </div>
</div>
</template>

<script lang="ts" setup>

</script>

<style>

</style>