<div class="container"><slot /></div>

<style>
  .container {
    max-width: 1200px;
    margin: 0 auto;
  }

  @media (max-width: 1200px) {
    .container {
      width: 100%;
      padding: 0 1rem;
    }
  }

  @media (max-width: 768px) {
    .container {
      width: 100%;
      padding: 0 0.5rem;
    }
  }
</style>
