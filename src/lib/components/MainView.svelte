<script lang="ts">
  import Name from './Name.svelte';
  import NeuralNet from './NeuralNet.svelte';
  import ScrollIcon from './ScrollIcon.svelte';
</script>

<section>
  <Name />
  <NeuralNet />
  <ScrollIcon />
</section>

<style>
  section {
    display: flex;
    height: 100vh;
    max-width: 1200px;
  }

  :global(.ml15) {
    color: #fff;
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  :global(.neural-net) {
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  @media (max-width: 768px) {
    section {
      width: 100%;
      flex-direction: column;
      justify-content: center;
      align-items: center;
    }

    :global(.ml15) {
      color: #fff;
      width: 300px;
      display: flex;
    }

    :global(.ml15 .word) {
      font-size: 80px;
      display: block;
      line-height: 1em;
      margin-bottom: 2.5em;
    }

    :global(.neural-net) {
      position: absolute;
      margin-top: 150px;
      width: 300px;
      height: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
    }
  }
</style>
