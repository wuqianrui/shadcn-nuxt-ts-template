<template>
<div>
  <div class="preview flex min-h-[50px] w-full justify-center p-10 items-center">
    <a href="https://www.shadcn-vue.com/docs/components/calendar"  target="_blank" class="text-blue-500 hover:underline">component docs</a>
    <div class="w-8"/>
    <a href="https://www.radix-vue.com/components/calendar.html"  target="_blank" class="text-blue-500 hover:underline">api docs</a>
  </div>
  <div class="preview flex min-h-[50px] w-auto justify-center p-10 items-center space-x-4 bg-gray-100 rounded-lg mx-10">
    <!-- fill component -->
    <div >
    <UiCalendar v-model="value" locale='en' :weekday-format="'short'" calendar-label="Date of birth" class="rounded-md border bg-green-50"  />
    </div>
    <!-- fill component -->
  </div>
  <div  class="preview flex w-auto justify-center p-10 items-center mx-10">
    use <a href="https://react-spectrum.adobe.com/internationalized/date/index.html" target="_blank" class="text-blue-500 mx-2">@internationalized/date</a> package, solves a lot of the problems that come with working with dates and times in JavaScript .
  </div>
</div>
</template>

<script lang="ts" setup>
import { type Ref, ref } from 'vue'
import { type DateValue, getLocalTimeZone, today } from '@internationalized/date'

const value = ref(today(getLocalTimeZone())) as Ref<DateValue>
</script>

<style>

</style>