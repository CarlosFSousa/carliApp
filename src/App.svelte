<script>
  // @ts-nocheck
  import { onMount } from 'svelte';
  const countDownDate = new Date('Jul 8, 2023 00:00:00').getTime();
  onMount(() => {
    const now = new Date().getTime();
    const timeleft = countDownDate - now;
    const days = Math.floor(timeleft / (1000 * 60 * 60 * 24));
    document.getElementById('days').innerHTML = String(days);
  });
</script>

<main>
  <div>
    <nav class="navbar navbar-expand-lg bg-light">
      <div class="container-fluid">
        <a class="navbar-brand" href="#">Carlos&Ali</a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon" />
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#">Home</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Link</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Link</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>

    <div class="main-text" align="center">
      <h4>Welcome to</h4>
      <h1>Carlos & Ali's</h1>
      <h4>official wedding website</h4>
    </div>
    <div class="main-countdown" align="center">
      <div class="countdown">
        <h4>Coutdown to our big day</h4>
        <div><span id="days">260</span><span>days</span></div>
      </div>
    </div>
  </div>
</main>

<style>
  .main-text {
    margin-top: 6em;
  }

  .main-text > h1 {
    font-size: 3em;
  }

  .days {
    font-size: 10rem;
  }

  * {
    font-family: 'Merchant';
  }

  .countdown {
    width: 50%;
    border-radius: 25%;
    background-color: grey;
    margin: 1em;
    padding: 2em;
  }
</style>
