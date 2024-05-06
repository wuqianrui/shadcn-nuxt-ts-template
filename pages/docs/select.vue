<template>
<div>
  <div class="preview flex min-h-[50px] w-full justify-center p-10 items-center">
    <a href="https://www.shadcn-vue.com/docs/components/select.html"  target="_blank" class="text-blue-500 hover:underline">shadcn-vue docs</a>
    <div class="w-8"/>
    <a href="https://www.radix-vue.com/components/select#root"  target="_blank" class="text-blue-500 hover:underline">api docs</a>
  </div>
  <div class="preview flex min-h-[50px] w-auto justify-center p-10 items-center space-x-4 bg-blue-100 rounded-lg mx-10">
    <!-- 这里填写组件 -->
     <UiSelect>
    <UiSelectTrigger class="w-[280px]">
      <UiSelectValue placeholder="UiSelect a timezone" />
    </UiSelectTrigger>
    <UiSelectContent>
      <UiSelectGroup>
        <UiSelectLabel>North America</UiSelectLabel>
        <UiSelectItem value="est">
          Eastern Standard Time (EST)
        </UiSelectItem>
        <UiSelectItem value="cst">
          Central Standard Time (CST)
        </UiSelectItem>
        <UiSelectItem value="mst">
          Mountain Standard Time (MST)
        </UiSelectItem>
        <UiSelectItem value="pst">
          Pacific Standard Time (PST)
        </UiSelectItem>
        <UiSelectItem value="akst">
          Alaska Standard Time (AKST)
        </UiSelectItem>
        <UiSelectItem value="hst">
          Hawaii Standard Time (HST)
        </UiSelectItem>
      </UiSelectGroup>
      <UiSelectGroup>
        <UiSelectLabel>Europe & Africa</UiSelectLabel>
        <UiSelectItem value="gmt">
          Greenwich Mean Time (GMT)
        </UiSelectItem>
        <UiSelectItem value="cet">
          Central European Time (CET)
        </UiSelectItem>
        <UiSelectItem value="eet">
          Eastern European Time (EET)
        </UiSelectItem>
        <UiSelectItem value="west">
          Western European Summer Time (WEST)
        </UiSelectItem>
        <UiSelectItem value="cat">
          Central Africa Time (CAT)
        </UiSelectItem>
        <UiSelectItem value="eat">
          East Africa Time (EAT)
        </UiSelectItem>
      </UiSelectGroup>
      <UiSelectGroup>
        <UiSelectLabel>Asia</UiSelectLabel>
        <UiSelectItem value="msk">
          Moscow Time (MSK)
        </UiSelectItem>
        <UiSelectItem value="ist">
          India Standard Time (IST)
        </UiSelectItem>
        <UiSelectItem value="cst_china">
          China Standard Time (CST)
        </UiSelectItem>
        <UiSelectItem value="jst">
          Japan Standard Time (JST)
        </UiSelectItem>
        <UiSelectItem value="kst">
          Korea Standard Time (KST)
        </UiSelectItem>
        <UiSelectItem value="ist_indonesia">
          Indonesia Central Standard Time (WITA)
        </UiSelectItem>
      </UiSelectGroup>
      <UiSelectGroup>
        <UiSelectLabel>Australia & Pacific</UiSelectLabel>
        <UiSelectItem value="awst">
          Australian Western Standard Time (AWST)
        </UiSelectItem>
        <UiSelectItem value="acst">
          Australian Central Standard Time (ACST)
        </UiSelectItem>
        <UiSelectItem value="aest">
          Australian Eastern Standard Time (AEST)
        </UiSelectItem>
        <UiSelectItem value="nzst">
          New Zealand Standard Time (NZST)
        </UiSelectItem>
        <UiSelectItem value="fjt">
          Fiji Time (FJT)
        </UiSelectItem>
      </UiSelectGroup>
      <UiSelectGroup>
        <UiSelectLabel>South America</UiSelectLabel>
        <UiSelectItem value="art">
          Argentina Time (ART)
        </UiSelectItem>
        <UiSelectItem value="bot">
          Bolivia Time (BOT)
        </UiSelectItem>
        <UiSelectItem value="brt">
          Brasilia Time (BRT)
        </UiSelectItem>
        <UiSelectItem value="clt">
          Chile Standard Time (CLT)
        </UiSelectItem>
      </UiSelectGroup>
    </UiSelectContent>
  </UiSelect>
    <!-- 这里填写组件 -->
  </div>
</div>
</template>

<script lang="ts" setup>

</script>

<style>

</style>