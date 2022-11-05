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
      <p class="greeting">Welcome to</p>
      <p class="names">CARLOS & ALI'S</p>
      <p class="greeting">official wedding website</p>
    </div>
  </div>
  <div class="main-countdown">
    <div class="countdown">
      <p>Coutdown to our big day</p>
      <div><span id="days" /><span class="days">days</span></div>
    </div>
  </div>
</main>

<style>
  p {
    margin: 0;
  }
  .main-text {
    padding-top: 8em;
  }

  .greeting {
    font-size: 2em;
  }

  .names {
    font-size: 90px;
  }
  .countdown {
    border-radius: 20%;
    background-color: #c6cdc0;
    text-align: center;
    margin: 0 auto;
    padding: 1em;
    width: 35%;
  }

  .text {
    text-align: center;
  }

  #days {
    font-size: 8em;
  }

  .days {
    font-size: 1em;
  }

  .main-countdown {
    margin: 2em;
  }

  .countdown > p {
    font-size: 1.5em;
    width: 40%;
    margin: 0 auto;
  }

  @media (max-width: 480px) {
    #days {
      font-size: 100px;
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
    color: #350101;
    font-style: normal;
    font-weight: 100;
    letter-spacing: -1px;
  }
</style>
