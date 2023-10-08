<script lang="ts">
</script>

<section>
  <h1>Works & Activity</h1>
  <div class="cards">
    <div class="card">
      <h3>Beach Litter API</h3>
      <p>
        API to identify beach litter and a front end to use the API are constructed.
        The API was created using Svelte and Python.
      </p>
    </div>
    <div class="card">
      <h3>Portfolio</h3>
      <p>
        This portfolio is built with Svelte and Vercel.
        Also, use anime.js to animate the page.
        <br>
        <a href="https://github.com/fightingsou/portfolio">GitHub</a>
      </p>
    </div>
    <div class="card">
      <h3>TCU R-Presco</h3>
      <p>
        Presentation on "Mosaic Art Generation by Symbiotic Evolution" at Tokyo City University Research Presentation Contest.
        Received an award for excellence.
        <br>
        <a href="https://informatics.tcu.ac.jp/news/award/?&p=841">Article</a>
      </p>
    </div>
  </div>

  <div class="cards">
    <div class="card">
      <h3>GitHub Training Seminar</h3>
      <p>
        I taught about 50 juniors the basics of how GitHub works and how to use it.
        <br>
        <a href="https://speakerdeck.com/fightingsou/githubjiang-xi-hui-2023">Slide</a>
      </p>
    </div>
    <div class="card">
      <h3>The Thinker</h3>
      <p>
        Developed a Vue application for a research project in a university course "Problem-Based Learning through Sustainable Development Project".
Won 3rd place out of about 300 teams.
      </p>
    </div>
  </div>

</section>

<style>
  section {
    height: 100vh;
    max-width: 1200px;
    margin: 0 auto;
  }

  h1 {
    font-size: 6rem;
    font-family: 'Sacramento', cursive;
    color: #aaa;
    text-align: center;
    padding-top: 10vh;
  }

  .cards {
    display: flex;
    justify-content: space-around;
  }

  .card {
    border: 1px solid #aaa;
    border-radius: 20px;
    padding: 2rem;
    margin: 0 auto;
    margin-top: 3vh;
    width: 300px;
    height: 400px;
  }

  h3 {
    font-size: 2rem;
    font-family: 'Sacramento', cursive;
    color: #aaa;
    text-align: center;
  }

  p {
    font-size: 1.0rem;
    font-family: 'Alegreya Sans', sans-serif;
    color: #aaa;
    text-align: center;
    max-width: 80vw;
    margin: 0 auto;
    margin-top: 3vh;
  }

  a {
    font-size: 1.0rem;
    font-family: 'Alegreya Sans', sans-serif;
    text-align: center;
    text-decoration: none;
    max-width: 80vw;
    margin: 0 auto;
  }

  @media screen and (max-width: 600px) {
    h1 {
      font-size: 4rem;
      padding-top: 30vh;
      margin: 0 auto;
    }

    .cards {
      flex-direction: column;
      align-items: center;
    }

    .card {
      height: 300px;
    }

    p {
      font-size: 0.8rem;
    }

    a {
      font-size: 0.8rem;
    }
  }
</style>

