<template>
<div>
  <div class="preview flex min-h-[50px] w-full justify-center p-10 items-center">
    <a href="https://www.shadcn-vue.com/docs/components/popover"  target="_blank" class="text-blue-500 hover:underline">component docs</a>
    <div class="w-8"/>
    <a href="https://www.radix-vue.com/components/popover.html"  target="_blank" class="text-blue-500 hover:underline">api docs</a>
  </div>
  <div class="preview flex min-h-[50px] w-auto justify-center p-10 items-center space-x-4 bg-gray-100 rounded-lg mx-10">
    <!-- fill component -->
  <UiPopover>
    <UiPopoverTrigger as-child>
      <UiButton variant="outline">
        Open UiPopover
      </UiButton>
    </UiPopoverTrigger>
    <UiPopoverContent class="w-80">
      <div class="grid gap-4">
        <div class="space-y-2">
          <h4 class="font-medium leading-none">
            Dimensions
          </h4>
          <p class="text-sm text-muted-foreground">
            Set the dimensions for the layer.
          </p>
        </div>
        <div class="grid gap-2">
          <div class="grid grid-cols-3 items-center gap-4">
            <UiLabel for="width">Width</UiLabel>
            <UiInput
              id="width"
              type="text"
              default-value="100%"
              class="col-span-2 h-8"
            />
          </div>
          <div class="grid grid-cols-3 items-center gap-4">
            <UiLabel for="maxWidth">Max. width</UiLabel>
            <UiInput
              id="maxWidth"
              type="text"
              default-value="300px"
              class="col-span-2 h-8"
            />
          </div>
          <div class="grid grid-cols-3 items-center gap-4">
            <UiLabel for="height">Height</UiLabel>
            <UiInput
              id="height"
              type="text"
              default-value="25px"
              class="col-span-2 h-8"
            />
          </div>
          <div class="grid grid-cols-3 items-center gap-4">
            <UiLabel for="maxHeight">Max. height</UiLabel>
            <UiInput
              id="maxHeight"
              type="text"
              default-value="none"
              class="col-span-2 h-8"
            />
          </div>
        </div>
      </div>
    </UiPopoverContent>
  </UiPopover>
    <!-- fill component -->
  </div>
</div>
</template>

<script lang="ts" setup>

</script>

<style>

</style>