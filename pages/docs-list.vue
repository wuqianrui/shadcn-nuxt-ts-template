<template>
  <div>
    <!-- <div v-for="item in docsList" :key="item">
        <NuxtLink :to="'/docs/'+item" class="min-h-[50px]">{{item}}</NuxtLink>
    </div> -->

    <ul class="my-6 ml-6 list-disc [&>li]:mt-2">
      <li v-for="item in docsList" :key="item" class="hover:underline">
        <NuxtLink :to="'/docs/'+item.path" class="min-h-[50px]">{{item.name}}</NuxtLink>
      </li>
    </ul>

  <br/>
    
  
  </div>

</template>

<script lang="ts" setup>

  const docsList = [
    {"path":"accordion","name":"accordion ✅"},{"path":"alert","name":"alert ✅"},
  {"path":"alert-dialog","name":"alert-dialog ✅"},{"path":"aspect-ratio","name":"aspect-ratio ✅"},
  {"path":"avatar","name":"avatar ✅"},{"path":"badge","name":"badge ✅"},{"path":"breadcrumb","name":"breadcrumb ✅"},
  {"path":"button","name":"button ✅"},{"path":"calendar","name":"calendar"},{"path":"card","name":"card"},
  {"path":"carousel","name":"carousel ✅"},{"path":"checkbox","name":"checkbox ✅"},{"path":"collapsible","name":"collapsible"},
  {"path":"combobox","name":"combobox"},{"path":"command","name":"command"},{"path":"context-menu","name":"context-menu"},
  {"path":"data-table","name":"data-table"},{"path":"date-picker","name":"date-picker"},{"path":"dialog","name":"dialog"},
  {"path":"divider","name":"divider ✅"},{"path":"drawer","name":"drawer"},{"path":"dropdown-menu","name":"dropdown-menu"},{"path":"form","name":"form"},
  {"path":"hover-card","name":"hover-card ✅"},{"path":"input","name":"input"},{"path":"label","name":"label ✅"},
  {"path":"menubar","name":"menubar"},{"path":"navigation-menu","name":"navigation-menu"},
  {"path":"pagination","name":"pagination"},{"path":"pin-input","name":"pin-input"},
  {"path":"popover","name":"popover"},{"path":"progress","name":"progress"},{"path":"radio-group","name":"radio-group"},
  {"path":"range-calendar","name":"range-calendar"},{"path":"resizable","name":"resizable"},{"path":"scroll-area","name":"scroll-area"},
  {"path":"select","name":"select ✅"},{"path":"separator","name":"separator ✅"},{"path":"sheet","name":"sheet"},
  {"path":"skeleton","name":"skeleton"},{"path":"slider","name":"slider"},{"path":"sonner","name":"sonner"},
  {"path":"switch","name":"switch"},{"path":"table","name":"table"},{"path":"tabs","name":"tabs"},
  {"path":"tags-input","name":"tags-input"},{"path":"textarea","name":"textarea"},{"path":"toast","name":"toast"},
  {"path":"toggle","name":"toggle"},{"path":"toggle-group","name":"toggle-group"},
  {"path":"tooltip","name":"tooltip"},
  {"path":"tool-lucide","name":"🛠️ Lucide Icon"},
  {"path":"dropfile","name":"Ui-Thing Dropfile"},
  {"path":"chip","name":"🪼 Nuxt UI Chip"}
  ]
  
</script>
<style>

</style>