<template>
<div>
  <div class="preview flex min-h-[50px] w-full justify-center p-10 items-center">
    <a href="https://www.shadcn-vue.com/docs/components/breadcrumb.html"  target="_blank">shadcn-vue docs</a>
  </div>
  <div class="preview flex min-h-[50px] w-auto justify-center p-10 items-center space-x-4 bg-gray-100 rounded-lg mx-10">
    <!-- 这里填写组件 -->
     <UiBreadcrumb>
    <UiBreadcrumbList>
      <UiBreadcrumbItem>
        <UiBreadcrumbLink href="/">
          Home
        </UiBreadcrumbLink>
      </UiBreadcrumbItem>
      <UiBreadcrumbSeparator/>
      <UiBreadcrumbItem>
        <UiBreadcrumbLink href="/test">
          Components
        </UiBreadcrumbLink>
      </UiBreadcrumbItem>
      <UiBreadcrumbSeparator/>
      <UiBreadcrumbItem>
        <UiBreadcrumbPage>UiBreadcrumb</UiBreadcrumbPage>
      </UiBreadcrumbItem>
    </UiBreadcrumbList>
  </UiBreadcrumb>
    <!-- 这里填写组件 -->
  </div>

   <div class="preview flex min-h-[50px] w-auto justify-center p-10 items-center space-x-4 bg-gray-100 rounded-lg mx-10">
    <!-- 这里填写组件 -->
     <UiBreadcrumb>
    <UiBreadcrumbList>
      <UiBreadcrumbItem>
        <UiBreadcrumbLink href="/">
          Home
        </UiBreadcrumbLink>
      </UiBreadcrumbItem>
      <UiBreadcrumbSeparator>
        <Slash/>
      </UiBreadcrumbSeparator>
      <UiBreadcrumbItem>
        <UiBreadcrumbLink href="/test">
          Components
        </UiBreadcrumbLink>
      </UiBreadcrumbItem>
      <UiBreadcrumbSeparator>
        <Slash/>
      </UiBreadcrumbSeparator>
      <UiBreadcrumbItem>
        <UiBreadcrumbPage>UiBreadcrumb</UiBreadcrumbPage>
      </UiBreadcrumbItem>
    </UiBreadcrumbList>
  </UiBreadcrumb>
    <!-- 这里填写组件 -->
  </div>

    官方文档需要补充！！！

</div>
</template>

<script lang="ts" setup>
import { ChevronDown, Slash } from 'lucide-vue-next'
</script>

<style>

</style>