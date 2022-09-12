<script>
	import { Button, Heading, Mark, Span, P, Label, Iconinput } from 'flowbite-svelte';
  import { slide, fade, fly } from 'svelte/transition';
  import { onMount } from 'svelte';
  import { cubicInOut, sineInOut } from 'svelte/easing';

  let ready = false;
  onMount(() => ready = true);
</script>

{#if ready}
<div in:slide="{{ easing: cubicInOut, duration: 1500 }}" out:slide>
  <h1 class="gamer">
    bbot-r
  </h1>
  <p>
    bbot, reimagined.
  </p>
  <p class="seperator">‎ </p>
  <hr />
  <p class="seperator">‎ </p>
  <button>script</button>
</div>
{/if}