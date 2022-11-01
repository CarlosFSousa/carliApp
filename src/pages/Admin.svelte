<script>
  import { onMount } from 'svelte';

  const userLoggedIn = false;
</script>

<main>
  {#if userLoggedIn}
    <h1>Admin</h1>
  {:else}
    <h1>You need to login</h1>
  {/if}
</main>
