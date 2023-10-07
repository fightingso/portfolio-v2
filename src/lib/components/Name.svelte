<script>
  import { onMount } from 'svelte';
  import anime from 'animejs';

  let text;

  onMount(() => {
    anime.timeline({loop: false})
      .add({
        targets: '.ml15 .word',
        scale: [14,1],
        opacity: [0,1],
        easing: "easeOutCirc",
        duration: 800,
        delay: (el, i) => 800 * i
      }).add({
        targets: '.ml15',
        opacity: 1,
        duration: 1000,
        easing: "easeOutExpo",
        delay: 1000
      });

    text.addEventListener('mouseover', () => {
      anime({
        targets: text,
        scale: 1.1,
        direction: 'alternate',
        loop: true,
        easing: 'easeInOutSine',
      });
    });

    text.addEventListener('mouseout', () => {
      anime.remove(text);
      text.style.transform = 'scale(1)';
    });
  });
</script>

<style>
  .ml15 {
    font-size: 10em;
    width: 1000px;
    white-space: nowrap;
  }

  .ml15 .word {
    font-family: 'Sacramento', cursive;
    color: #aaa;
    display: inline-block;
    line-height: 1em;
  }

  @media (max-width: 768px) {
    .ml15 {
      width: 400px;
    }
  }
</style>

<div class="ml15" bind:this={text}>
  <span class="word">So</span>
  <span class="word">Hirawata</span>
</div>

