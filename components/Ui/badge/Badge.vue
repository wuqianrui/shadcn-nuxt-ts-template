<script setup lang="ts">
import { computed } from "vue";
import { cva } from "class-variance-authority";
import { cn } from "@/lib/utils";

interface BadgeProps {
  variant?: "primary" | "secondary" | "outline" | "destructive" | 'success' | 'warning' | 'danger';
  as?: string;
  class?: string;
}

const props = withDefaults(defineProps<BadgeProps>(), {
  variant: "primary",
  as: "span",
});

const badgeClass = computed(() => {
  return cva(
    "inline-flex items-center cursor-default text-xs font-semibold px-2.5 py-0.5 rounded-full transition-colors ease-in-out duration-300",
    {
      variants: {
        variant: {
          primary: "bg-primary text-primary-foreground",
          secondary: "bg-secondary text-foreground",
          outline: "border border-border text-foreground shadow-sm",
          destructive: "bg-destructive text-destructive-foreground",
          success: 'dark:border-emerald-600 dark:text-emerald-400 dark:bg-emerald-900/50 border-emerald-500 text-emerald-500 bg-emerald-400/20',
        warning: 'dark:border-amber-500 dark:text-amber-500 dark:bg-amber-900/50 border-amber-500 text-amber-500 bg-amber-400/20',
        danger: 'dark:border-red-500 dark:text-red-500 dark:bg-red-900/50 border-red-500 text-red-500 bg-red-400/20',
        },
      },
    },
  )({
    variant: props.variant,
  });
});
</script>

<template>
  <component :is="props.as" :class="cn(badgeClass, props.class)">
    <slot />
  </component>
</template>
