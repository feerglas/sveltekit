<script>
import { onMount } from 'svelte';

onMount(async () => {
  const lyne = await import(/* @vite-ignore */'lyne-test/dist/custom-elements');

  lyne.defineCustomElements();
});
</script>

<lyne-cta-button label="button"></lyne-cta-button>
