<script>
  // @ts-nocheck
  import { Route, Router } from 'svelte-navigator';
  import Azores from './pages/Azores.svelte';
  import Expectations from './pages/Expectations.svelte';
  import Home from './pages/Home.svelte';
  import Navbar from './pages/Navbar.svelte';
  import NotFound from './pages/NotFound.svelte';
  import Tips from './pages/Tips.svelte';
  import WhereAndWhen from './pages/WhereAndWhen.svelte';
</script>

<main>
  <Router>
    <Navbar />
    <Route path="/"><Home /></Route>
    <Route path="/whereandwhen"><WhereAndWhen /></Route>
    <Route path="/expectations"><Expectations /></Route>
    <Route path="/tips"><Tips /></Route>
    <Route path="/azores"><Azores /></Route>
    <Route path="/:notfound"><NotFound /></Route>
  </Router>
</main>

<style>
</style>
