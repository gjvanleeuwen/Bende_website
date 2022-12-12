<script lang="ts">

  import Header from "./assets/header.svelte";
  import Footer from "./assets/footer.svelte";
  import Banner from "./assets/banner.svelte";
  import Services from "./assets/services.svelte";

  import Youtube from "svelte-youtube-embed";



</script>

<Header />
<Banner/>

<Services/>
<main>

  <div>
    <a href="/" target="_blank" rel="noreferrer">
      <img src="/logo_transparant.png" class="logo" alt="Bende logo" />
    </a>
  </div>
</main>

<Footer />

<style>
  .logo-small {
    height: 2em;
    padding: 1.5em;
    will-change: filter;
  }
  .logo {
    height: 6em;
    padding: 1.5em;
    will-change: filter;
  }
  .logo:hover {
    filter: drop-shadow(0 0 2em #646cffaa);
  }

  .grey-text {
    color: #888;
  }
</style>