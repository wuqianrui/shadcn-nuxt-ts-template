<template>
<div>
  <div class="preview flex min-h-[50px] w-full justify-center p-10 items-center">
    <a href="https://ui-thing.behonbaker.com/components/dropfile#placeholder"  target="_blank" class="text-blue-500 hover:underline">ui-thing component docs</a>
    <div class="w-8"/>
    <a href="https://github.com/BayBreezy/ui-thing/tree/main/components/Ui/Dropfile.vue"  target="_blank" class="text-blue-500 hover:underline">api docs</a>
  </div>
  <div class="preview flex flex-col min-h-[50px] w-auto justify-center p-10 items-center space-x-4 bg-gray-100 rounded-lg mx-10">
    <!-- fill component -->
    <UiDropfile @dropped="files = $event" />
    <div class="mt-5" v-if="files && files.length">
      <div
        v-for="(file, i) in files"
        :key="file.name"
        class="group relative mb-2 flex h-12 items-center justify-between rounded border px-3 py-3"
      >
        <div class="flex grow items-center gap-3">
          <Icon name="heroicons:document" class="mr-3 h-8 w-8 opacity-60" />
          <p class="w-[80%] truncate text-sm">{{ file.name }}</p>
          <p
            class="hidden group-hover:block ml-auto whitespace-nowrap text-xs mr-3 text-muted-foreground/60 transition"
          >
            {{ formatFileSize(file.size) }}
          </p>
        </div>

        <div class="">
          <UiButton @click="removeFile(i)" size="icon-sm" variant="outline">
            <Icon name="heroicons:x-mark" class="h-3.5 w-3.5" />
          </UiButton>
        </div>
      </div>
    </div>
    <!-- fill component -->
  </div>
</div>
</template>

<script lang="ts" setup>
const files = ref<File[]>([]);

function formatFileSize(fileSize:number) {
  if (fileSize === 0) return '0 B';
  const units = ['B', 'KB', 'MB', 'GB', 'TB', 'PB', 'EB', 'ZB', 'YB'];
  let i = 0;
  while (fileSize >= 1024) {
    fileSize /= 1024;
    i++;
  }
  return `${fileSize.toFixed(1)} ${units[i]}`;
}

function removeFile(index:number){
  console.log(index);
  if (index < 0 || index >= files.value.length) {
    return
  }
  files.value.splice(index, 1)
}

</script>

<style>

</style>