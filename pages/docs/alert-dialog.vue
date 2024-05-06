<template>
<div>
  <div class="preview flex min-h-[50px] w-full justify-center p-10 items-center">
    <a href="https://ui-thing.behonbaker.com/components/alertdialog#usage"  target="_blank">shadcn-vue docs</a>
  </div>
  <div class="preview flex min-h-[50px] w-auto justify-center p-10 items-center space-x-4 bg-gray-100 rounded-lg mx-10">
    <!-- 这里填写组件 -->
    <UiAlertDialog v-model:open="model">
      <UiAlertDialogTrigger as-child>
        <UiButton variant="outline">Show Dialog</UiButton>
      </UiAlertDialogTrigger>
      <UiAlertDialogContent @escape-key-down="showMessage('Escape key pressed')">
        <UiAlertDialogHeader>
          <UiAlertDialogTitle>Are you absolutely sure?</UiAlertDialogTitle>
          <UiAlertDialogDescription>
            This action cannot be undone. This will permanently delete your account and remove your
            data from our servers.
          </UiAlertDialogDescription>
        </UiAlertDialogHeader>
        <UiAlertDialogFooter>
          <UiAlertDialogCancel @click="closeDialog">
            <UiButton variant="ghost">cancel</UiButton>
          </UiAlertDialogCancel>
          <UiAlertDialogAction @click="closeDialog">
            <UiButton>Continue</UiButton>
          </UiAlertDialogAction>
        </UiAlertDialogFooter>
      </UiAlertDialogContent>
    </UiAlertDialog>
    <!-- 这里填写组件 -->
  </div>
</div>
</template>

<script lang="ts" setup>

const model = ref(false);

const closeDialog = ()=>{
  model.value = false
}
</script>

<style>

</style>