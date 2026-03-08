<script lang="ts">
  type Props = {
    variant?: 'primary' | 'black';
    className?: string;
    onclick?: () => void;
    children?: import('svelte').Snippet;
  };

  let { variant = 'primary', className = '', onclick, children }: Props = $props();
</script>

<button 
  {onclick}
  class={[
    'inline-flex items-center justify-center gap-2.5 rounded-full px-8 py-4 text-base font-semibold',
    'transition-all duration-300 active:scale-95 hover:scale-105',
    'bg-gradient-to-br from-black via-gray-800 to-gray-900 text-white hover:from-gray-800 hover:via-gray-700 hover:to-gray-800 ring-1 ring-black/10',
    className
  ]}
>
  {@render children?.()}
</button>
