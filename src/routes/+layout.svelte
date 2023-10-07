<script>
  import "$lib/assets/styles/global.css";
  import MainView from "$lib/components/MainView.svelte";
  import Container from "$lib/components/Container.svelte";
  import Content from "$lib/components/Content.svelte";
  import Footer from "$lib/components/Footer.svelte";
</script>

<Container>
  <MainView />
  <Footer />
</Container>

<style>
  :global(html) {
    background-color: #111;
  }

  section {
    min-height: 100svh;
  }

  .Footer {
    position: absolute;
    bottom: 0;
    width: 100%;
  }
</style>
