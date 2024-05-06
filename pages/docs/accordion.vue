<template>
<div>
  <div class="preview flex min-h-[50px] w-full justify-center p-10 items-center">
    <a href="https://www.shadcn-vue.com/docs/components/accordion"  target="_blank" class="text-blue-500 hover:underline">component docs</a>
    <div class="w-8"/>
    <a href="https://www.radix-vue.com/components/accordion#api-reference"  target="_blank" class="text-blue-500 hover:underline">api docs</a>
  </div>
  <div class="preview flex min-h-[50px] w-auto justify-center p-10 items-center space-x-4 bg-gray-100 rounded-lg mx-10">
    <div class="bg-white px-4 py-2 rounded-md shadow-md min-w-[820px] ">
        <UiAccordion type="single" class="w-4/4" collapsible :default-value="defaultValue" >
    <UiAccordionItem v-for="item in accordionItems" :key="item.value" :value="item.value">
      <UiAccordionTrigger>{{ item.title }}</UiAccordionTrigger>
      <UiAccordionContent>
        {{ item.content }}
      </UiAccordionContent>
    </UiAccordionItem>
  </UiAccordion>
    </div>  
  </div>
</div>
</template>

<script lang="ts" setup>
  const accordionItems = [
    {
      value: "item-1",
      title: "Is it accessible?",
      content: "Yes. It adheres to the WAI-ARIA design pattern.",
    },
    {
      value: "item-2",
      title: "Is it unstyled?",
      content: "Yes. It's unstyled by default, giving you freedom over the look and feel.",
    },
    {
      value: "item-3",
      title: "Can it be animated?",
      content: "Yes! You can use the transition prop to configure the animation.",
    },
  ];
</script>

<style>

</style>