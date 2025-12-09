<script lang="ts">
  import { onMount } from 'svelte';
  
  export let variant: 'primary' | 'black' = 'primary';
  export let className = '';
</script>

<button 
  class="
    inline-flex items-center justify-center gap-2 rounded-full px-5 py-2.5 text-sm font-semibold transition-transform active:scale-95
    {variant === 'primary' ? 'bg-black text-white hover:bg-gray-800' : ''}
    {variant === 'black' ? 'bg-black text-white hover:bg-gray-800' : ''}
    {className}
  "
>
  <slot />
</button>
