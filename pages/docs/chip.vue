<template>
<div>
  <div class="preview flex min-h-[50px] w-full justify-center p-10 items-center">
    <a href="https://ui.nuxt.com/components/chip"  target="_blank" class="text-blue-500 hover:underline">component docs</a>
    <div class="w-8"/>
    <a href="https://ui.nuxt.com/components/chip"  target="_blank" class="text-blue-500 hover:underline">api docs</a>
  </div>
  <div class="preview flex min-h-[50px] w-auto justify-center p-10 items-center space-x-4 bg-gray-100 rounded-lg mx-10">
    <!-- fill component -->
    <!-- avatar 01 -->
    <UiChip size="md" position="bottom-left" variant="warning">
      <UiAvatar>
        <UiAvatarImage
      src="https://images.unsplash.com/photo-1492633423870-43d1cd2775eb?&w=128&h=128&dpr=2&q=80"
      alt="Colm Tuite"
      fallback="CT"
      :delay-ms="600"
    /> 
    </UiAvatar>
    </UiChip>
    
    <!-- avatar 02 -->
    <UiChip size="xl2" position="bottom-right" variant="danger">
    <UiAvatar>
        <UiAvatarImage
            src="https://images.unsplash.com/photo-1511485977113-f34c92461ad9?ixlib=rb-1.2.1&w=128&h=128&dpr=2&q=80"
            alt="Colm Tuite"
            fallback='ct'
            :delay-ms="600"
    /> 
        <UiAvatarFallback :delay-ms="600" >JD</UiAvatarFallback>
    </UiAvatar>
    </UiChip>
    <!-- avatar 03 -->
    <UiChip size="md" position="bottom-right" variant="success" text="99+">
      <UiAvatar>
        <UiAvatarImage
      src="https://avatars.githubusercontent.com/u/739984?v=4"
      alt="Colm Tuite"
      fallback="CT"
      :delay-ms="600"
    /> 
    </UiAvatar>
    </UiChip>
    <!-- avatar 04 -->
    <UiAvatar>
    <UiAvatarFallback>JD</UiAvatarFallback>
    </UiAvatar>
    <!-- fill component -->
  </div>

</div>
</template>

<script lang="ts" setup>

</script>

<style>

</style>