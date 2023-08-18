<script>
  import Cart from "./Cart.svelte";
  import Nav from "./Nav.svelte";
  import { cartOpen } from "./lib/flags_stores";
</script>

<Nav />

{#if $cartOpen}  
<Cart />
{/if}
