<script>
  // @ts-nocheck
  import Navbar from './pages/Navbar.svelte';
  import Home from './pages/Home.svelte';
  import WhereAndWhen from './pages/WhereAndWhen.svelte';
  import NotFound from './pages/NotFound.svelte';
  import Expectations from './pages/Expectations.svelte';
  import Tips from './pages/Tips.svelte';
  import Azores from './pages/Azores.svelte';
  import Admin from './pages/Admin.svelte';
  import { Router, Route } from 'svelte-navigator';
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
    <Route path="/admin"><Admin /></Route>
  </Router>
</main>

<style>
</style>
