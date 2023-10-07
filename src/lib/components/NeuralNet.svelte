<script>
  import { onMount } from 'svelte';
  import anime from 'animejs';

  onMount(() => {
    anime({
      targets: '.node',
      backgroundColor: ['#FFF', '#F00', '#FFF'],
      duration: 10,
      loop: true,
      easing: 'easeInOutSine',
      delay: anime.stagger(200)
    });

    anime({
      targets: '.edge',
      strokeDashoffset: [anime.setDashoffset, 0],
      duration: 800,
      loop: true,
      direction: 'alternate',
      easing: 'easeInOutSine',
      delay: anime.stagger(200)
    });
  });
</script>

<style>
  .network {
    position: relative;
    width: 600px;
    height: 400px;
  }
  .node {
    position: absolute;
    width: 20px;
    height: 20px;
    border-radius: 50%;
    fill: #aaa;
    opacity: 1.0;
  }
  .edge {
    stroke: #aaa;
    stroke-width: 2;
    fill: none;
    opacity: 0.3;
  }
</style>

<div class="neural-net">
<svg class="network" viewBox="0 -100 600 400">
    <circle cx="50" cy="50" r="10" class="node"></circle>
    <line x1="50" y1="50" x2="150" y2="0" class="edge"></line>
    <line x1="50" y1="50" x2="150" y2="100" class="edge"></line>
    <line x1="50" y1="50" x2="150" y2="200" class="edge"></line>
    <circle cx="50" cy="150" r="10" class="node"></circle>
    <line x1="50" y1="150" x2="150" y2="0" class="edge"></line>
    <line x1="50" y1="150" x2="150" y2="100" class="edge"></line>
    <line x1="50" y1="150" x2="150" y2="200" class="edge"></line>

    <circle cx="150" cy="0" r="10" class="node"></circle>
    <line x1="150" y1="0" x2="250" y2="-50" class="edge"></line>
    <line x1="150" y1="0" x2="250" y2="50" class="edge"></line>
    <line x1="150" y1="0" x2="250" y2="150" class="edge"></line>
    <line x1="150" y1="0" x2="250" y2="250" class="edge"></line>
    <circle cx="150" cy="100" r="10" class="node"></circle>
    <line x1="150" y1="100" x2="250" y2="-50" class="edge"></line>
    <line x1="150" y1="100" x2="250" y2="50" class="edge"></line>
    <line x1="150" y1="100" x2="250" y2="150" class="edge"></line>
    <line x1="150" y1="100" x2="250" y2="250" class="edge"></line>
    <circle cx="150" cy="200" r="10" class="node"></circle>
    <line x1="150" y1="200" x2="250" y2="-50" class="edge"></line>
    <line x1="150" y1="200" x2="250" y2="50" class="edge"></line>
    <line x1="150" y1="200" x2="250" y2="150" class="edge"></line>
    <line x1="150" y1="200" x2="250" y2="250" class="edge"></line>

    <circle cx="250" cy="-50" r="10" class="node"></circle>
    <line x1="250" y1="-50" x2="350" y2="-50" class="edge"></line>
    <line x1="250" y1="-50" x2="350" y2="50" class="edge"></line>
    <line x1="250" y1="-50" x2="350" y2="150" class="edge"></line>
    <line x1="250" y1="-50" x2="350" y2="250" class="edge"></line>
    <circle cx="250" cy="50" r="10" class="node"></circle>
    <line x1="250" y1="50" x2="350" y2="-50" class="edge"></line>
    <line x1="250" y1="50" x2="350" y2="50" class="edge"></line>
    <line x1="250" y1="50" x2="350" y2="150" class="edge"></line>
    <line x1="250" y1="50" x2="350" y2="250" class="edge"></line>
    <circle cx="250" cy="150" r="10" class="node"></circle>
    <line x1="250" y1="150" x2="350" y2="-50" class="edge"></line>
    <line x1="250" y1="150" x2="350" y2="50" class="edge"></line>
    <line x1="250" y1="150" x2="350" y2="150" class="edge"></line>
    <line x1="250" y1="150" x2="350" y2="250" class="edge"></line>
    <circle cx="250" cy="250" r="10" class="node"></circle>
    <line x1="250" y1="250" x2="350" y2="-50" class="edge"></line>
    <line x1="250" y1="250" x2="350" y2="50" class="edge"></line>
    <line x1="250" y1="250" x2="350" y2="150" class="edge"></line>
    <line x1="250" y1="250" x2="350" y2="250" class="edge"></line>

    <circle cx="350" cy="-50" r="10" class="node"></circle>
    <line x1="350" y1="-50" x2="450" y2="-50" class="edge"></line>
    <line x1="350" y1="-50" x2="450" y2="50" class="edge"></line>
    <line x1="350" y1="-50" x2="450" y2="150" class="edge"></line>
    <line x1="350" y1="-50" x2="450" y2="250" class="edge"></line>
    <circle cx="350" cy="50" r="10" class="node"></circle>
    <line x1="350" y1="50" x2="450" y2="-50" class="edge"></line>
    <line x1="350" y1="50" x2="450" y2="50" class="edge"></line>
    <line x1="350" y1="50" x2="450" y2="150" class="edge"></line>
    <line x1="350" y1="50" x2="450" y2="250" class="edge"></line>
    <circle cx="350" cy="150" r="10" class="node"></circle>
    <line x1="350" y1="150" x2="450" y2="-50" class="edge"></line>
    <line x1="350" y1="150" x2="450" y2="50" class="edge"></line>
    <line x1="350" y1="150" x2="450" y2="150" class="edge"></line>
    <line x1="350" y1="150" x2="450" y2="250" class="edge"></line>
    <circle cx="350" cy="250" r="10" class="node"></circle>
    <line x1="350" y1="250" x2="450" y2="-50" class="edge"></line>
    <line x1="350" y1="250" x2="450" y2="50" class="edge"></line>
    <line x1="350" y1="250" x2="450" y2="150" class="edge"></line>
    <line x1="350" y1="250" x2="450" y2="250" class="edge"></line>

    <circle cx="450" cy="-50" r="10" class="node"></circle>
    <line x1="450" y1="-50" x2="550" y2="100" class="edge"></line>
    <circle cx="450" cy="50" r="10" class="node"></circle>
    <line x1="450" y1="50" x2="550" y2="100" class="edge"></line>
    <circle cx="450" cy="150" r="10" class="node"></circle>
    <line x1="450" y1="150" x2="550" y2="100" class="edge"></line>
    <circle cx="450" cy="250" r="10" class="node"></circle>
    <line x1="450" y1="250" x2="550" y2="100" class="edge"></line>

    <circle cx="550" cy="100" r="10" class="node"></circle>
  </svg>
</div>
