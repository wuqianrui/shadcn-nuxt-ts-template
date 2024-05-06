<template>
<div>
  <div class="preview flex min-h-[50px] w-full justify-center p-10 items-center">
    <a href="https://www.shadcn-vue.com/docs/components/checkbox"  target="_blank" class="text-blue-500 hover:underline">component docs</a>
    <div class="w-8"/>
    <a href="https://www.radix-vue.com/components/checkbox.html"  target="_blank" class="text-blue-500 hover:underline">api docs</a>
  </div>
  <div class="preview flex min-h-[50px] w-auto justify-center p-10 items-center space-x-4 bg-gray-100 rounded-lg mx-10">
    <!-- fill component -->

    <!-- 正常样式 -->
    <div class="items-top flex gap-x-2">
    <UiCheckbox id="terms1" @update:checked="checkCallback" />
    <div class="grid gap-1.5 leading-none">
      <Uilabel
        for="terms1"
        class="text-sm font-medium leading-none peer-disabled:cursor-not-allowed peer-disabled:opacity-70"
      >
        Accept terms and conditions
      </Uilabel>
      <p class="text-sm text-muted-foreground">
        You agree to our Terms of Service and Privacy Policy.
      </p>
    </div>
    </div>
    <br/>
    <hr/>
    <!-- 无法点击 -->
    
    <div class="items-top flex space-x-2">
    <UiCheckbox id="terms2" disabled />
    <label
      for="terms2"
      class="text-sm font-medium leading-none peer-disabled:cursor-not-allowed peer-disabled:opacity-70"
    >
      Accept terms and conditions
    </label>
  </div>

    <!-- 无法点击 -->
    
    <!-- fill component -->
  </div>
</div>
</template>

<script lang="ts" setup>
function checkCallback(val:Boolean){
  console.log("checked log",val)
}
</script>

<style>

</style>