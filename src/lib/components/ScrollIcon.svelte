<script>
  import { onMount } from "svelte";
  import anime from "animejs";

  let arrow;

  onMount(() => {
    // 矢印の上下移動のアニメーション
    anime({
      targets: arrow,
      translateY: [-10, 10],
      direction: "alternate",
      loop: true,
      easing: "easeInOutSine",
      duration: 1000,
    });
  });
</script>

<style>
  .container {
    position: fixed;
    bottom: 0;
    left: 50%;
    z-index: 100;
    margin-bottom: 2rem;
  }

  .arrow {
    font-size: 2rem;
    color: #eee;
    cursor: pointer;
  }
</style>

<div class="container">
  <div class="arrow" bind:this={arrow}>&#8595;</div>
</div>
