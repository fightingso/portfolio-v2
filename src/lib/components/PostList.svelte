<script lang="ts">
import { fade } from "svelte/transition";
</script>

<div class="post-list" in:fade={{ duration: 1000 }}>
  <slot />
</div>

<style>
.post-list {
  max-width: 700px;
  margin: 0 auto;
}
</style>
