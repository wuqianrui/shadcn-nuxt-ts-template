<template>
<div>
  <div class="preview flex min-h-[50px] w-full justify-center p-10 items-center">
    <a href="https://www.shadcn-vue.com/docs/components/alert.html">shadcn-vue docs</a>
  </div>
  <div class="preview flex min-h-[50px] w-full justify-center p-10 items-center">
    <UiAlert>
    <Terminal class="h-4 w-4" />
    <UiAlertTitle>Heads up!</UiAlertTitle>
    <UiAlertDescription>
      You can add components to your app using the cli.
    </UiAlertDescription>
  </UiAlert>
  </div>
  <div class="preview flex min-h-[50px] w-full justify-center p-10 items-center">
    <UiAlert variant="destructive">
    <UiAlertCircle class="w-4 h-4" />
    <UiAlertTitle>Error</UiAlertTitle>
    <UiAlertDescription>
      Your session has expired. Please log in again.
    </UiAlertDescription>
  </UiAlert>
  </div>
</div>
</template>

<script lang="ts" setup>
import { Terminal } from 'lucide-vue-next'
</script>

<style>

</style>