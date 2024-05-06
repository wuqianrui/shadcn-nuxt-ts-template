<template>
<div>
  <div class="preview flex min-h-[50px] w-full justify-center p-10 items-center">
    <a href="https://www.shadcn-vue.com/docs/components/toast"  target="_blank" class="text-blue-500 hover:underline">component docs</a>
    <div class="w-8"/>
    <a href="https://www.radix-vue.com/components/toast.html"  target="_blank" class="text-blue-500 hover:underline">api docs</a>
  </div>
  <div class="mx-10">
    Add the following Toaster component to your App.vue file !!!
  </div>
  <div class="min-h-[30px] min-w-[30px]" />

  <div class="preview flex min-h-[50px] w-auto justify-center p-10 items-center space-x-4 bg-gray-100 rounded-lg mx-10">
    <!-- 这里填写组件 -->
    <!-- <UiButton 
    variant="outline" @click="showToast">Add to calendar
   </UiButton>

   <UiButton 
    variant="outline" @click="showToastWithAction">with Action
   </UiButton>

   <UiButton 
    variant="outline" @click="showVariantToastWithAction">variant
   </UiButton>

   <UiButton 
    variant="outline" @click="showVariantToast('success')">success
   </UiButton>

   <UiButton 
    variant="outline" @click="showVariantToast('info')">info
   </UiButton>

   <UiButton 
    variant="outline" @click="showVariantToast('warning')">warning
   </UiButton>

    <UiButton 
    variant="outline" @click="showVariantToast('error')">error
   </UiButton> -->


    <!-- 这里填写组件 -->
  </div>
</div>
</template>

<script lang="ts" setup>
// import { toast , useToast } from '../../components/ui/toast/use-toast.ts'
// import { ToastAction } from '@/components/ui/toast'

// const { toast } = useToast()

// function showToast() {
//   toast({
//     title: 'Scheduled: Catch up',
//     description: 'Friday, February 10, 2023 at 5:57 PM',
//   })
// }

// function showToastWithAction(){
//   toast({
//         title: 'Uh oh! Something went wrong.',
//         description: 'There was a problem with your request.',
//         action: h(ToastAction, {
//           altText: 'Try again',
//         }, {
//           default: () => { return 'Try again' },
//         }),
//       });
// }

// function showVariantToastWithAction(){
//      toast({
//         title: 'Uh oh! Something went wrong.',
//         description: 'There was a problem with your request.',
//         variant: 'destructive',
//         action: h(ToastAction, {
//           altText: 'Try again',
//         }, {
//           default: () => { return 'Try again' },
//         }),
//       });
// }

// function showVariantToast(type:string){
//     toast({
//         title: 'Type of toast .',
//         description: 'There was a problem with your request.',
//         icon: getToasticon(type),
//         variant:   `${type}`,
//         action: h(ToastAction, {
//           altText: 'Try again',
//         }, {
//           default: () => { return 'Try again' },
//         }),
//       });
// }

// const getToasticon = (type: string) => {
//     switch (type) {
//       case "success":
//         return "lucide:badge-check";
//       case "info":
//         return "lucide:badge-info";
//       case "warning":
//         return "lucide:badge-alert";
//       case "destructive":
//         return "lucide:badge-x";
//       default:
//         return "lucide:badge-check";
//     }
//   };

</script>

<style>

</style>