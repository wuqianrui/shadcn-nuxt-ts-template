<script setup lang="ts">
import { computed } from "vue";
import { cva } from "class-variance-authority";
import { cn } from "@/lib/utils";

/**
 * source by Nuxt UI Chip 
 * docs: https://ui.nuxt.com/components/chip
 * github: 
 * https://github.com/nuxt/ui/blob/dev/src/runtime/components/elements/Chip.vue
 * https://github.com/nuxt/ui/blob/dev/src/runtime/ui.config/elements/chip.ts
*/

interface ChipProps {
  variant?: "primary" | "secondary" | "success" | "destructive" | "danger" | "warning" ;
  position?: "top-right" | "bottom-right" | "top-left" | "bottom-left";
  wrapper: boolean;
  text: string;
  size?: "xs" | "xs2" | "xs3" | "sm" | "md" | "lg" | "xl" | "xl2" | "xl3";
  class?: string;
}

const props = withDefaults(defineProps<ChipProps>(), {
  variant: "primary",
  size:"sm",
  wrapper:false
});

const chipClass = computed(() => {
  return cva(
    "absolute rounded-full ring-1 ring-white dark:ring-gray-900 flex items-center justify-center text-white dark:text-gray-900 font-medium whitespace-nowrap",
    {
      variants: {
        variant: {
          primary: "bg-primary",
          secondary: "bg-secondary",
          destructive: "bg-destructive",
          success: 'dark:bg-emerald-400 bg-emerald-500',
          warning: 'dark:bg-amber-400 bg-amber-500',
          danger: 'dark:bg-red-400 bg-red-500',
          
        },
        wrapper: {
            true: "inline-flex items-center justify-center flex-shrink-0",
        },
        position: {
            'top-right': 'top-0 right-0',
            'bottom-right': 'bottom-0 right-0',
            'top-left': 'top-0 left-0',
            'bottom-left': 'bottom-0 left-0'
        },
        // translate: {
        //     'top-right': '-translate-y-1/2 translate-x-1/2 transform',
        //     'bottom-right': 'translate-y-1/2 translate-x-1/2 transform',
        //     'top-left': '-translate-y-1/2 -translate-x-1/2 transform',
        //     'bottom-left': 'translate-y-1/2 -translate-x-1/2 transform'
        //   },
        size: {
            xs: 'h-1.5 min-w-[0.375rem] text-[6px] p-px',
            xs2: 'h-[5px] min-w-[5px] text-[5px] p-px',
            xs3: 'h-[4px] min-w-[4px] text-[4px] p-px',
            sm: 'h-2 min-w-[0.5rem] text-[7px] p-0.5',
            md: 'h-2.5 min-w-[0.625rem] text-[8px] p-0.5',
            lg: 'h-3 min-w-[0.75rem] text-[10px] p-0.5',
            xl: 'h-3.5 min-w-[0.875rem] text-[11px] p-1',
            xl2: 'h-4 min-w-[1rem] text-[12px] p-1',
            xl3: 'h-5 min-w-[1.25rem] text-[14px] p-1',

        },
        
      },
      defaultVariants: {
        variant: "primary",
        wrapper: false,
        position:"top-right",
        size: 'sm',
      },
    },
  )({
    variant: props.variant,
    position:props.position,
    size:props.size,
    wrapper:props.wrapper,
  });
});
</script>

<template>

    <div class="relative inline-flex items-center justify-center flex-shrink-0">
    <slot /> 
    
    <span :class="cn(chipClass, props.class)">
      <slot name="content">
        {{ text }}
      </slot>
    </span>
  </div>

</template>
