<script>
  import { onMount } from 'svelte';
  const countDownDate = new Date('Jul 8, 2023 00:00:00').getTime();
  onMount(() => {
    const now = new Date().getTime();
    const timeleft = countDownDate - now;
    const days = Math.floor(timeleft / (1000 * 60 * 60 * 24));
    document.getElementById('days').innerHTML = String(days);
  });
</script>

<main class="background">
  <div class="main-text">
    <div class="text">
      <h4>Welcome to</h4>
      <h1>Carlos & Ali's</h1>
      <h4>official wedding website</h4>
    </div>
  </div>
  <div class="main-countdown">
    <div class="countdown">
      <h4>Coutdown to our big day</h4>
      <div><span id="days" /><span>days</span></div>
    </div>
  </div>
</main>

<style>
  .main-text {
    padding-top: 16em;
  }

  h1 {
    font-size: 3em;
  }

  .countdown {
    border-radius: 40%;
    background-color: grey;
    text-align: center;
    margin: 0 auto;
    padding: 2em;
    width: 50%;
  }

  .text {
    text-align: center;
  }

  #days {
    font-size: 10em;
  }

  .main-countdown {
    margin: 2em;
  }

  @media (max-width: 480px) {
    #days {
      font-size: 2em;
    }

    .countdown {
      width: 100%;
    }
  }

  .background {
    background-image: url('../assets/background.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    height: 94vh;
  }
</style>
