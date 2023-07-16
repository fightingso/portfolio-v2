<script>
  import { MetaTags } from "svelte-meta-tags";
  import { envVariables } from "$lib/envVariables";
  import { blogMetaData } from "$lib/blogMetaData";
  import Awards from "$lib/components/Awards.svelte";
  import Papers from "$lib/components/Paper.svelte";

  const meta = {
    title: `About | ${blogMetaData.blogTitle}`,
    description: blogMetaData.description,
    url: envVariables.basePath,
    siteName: blogMetaData.blogTitle,
    image: {
      url: `${envVariables.basePath}/background.jpeg`,
      width: 1000,
      height: 523,
      alt: "image",
    },
  };
</script>

<MetaTags
  title={meta.title}
  description={meta.description}
  canonical={meta.url}
  openGraph={{
    description: meta.description,
    images: [
      {
        ...meta.image,
      },
    ],
    site_name: meta.siteName,
    title: meta.title,
    type: "website",
    url: meta.url,
  }}
  twitter={{
    cardType: "summary_large_image",
    title: meta.title,
    description: meta.description,
    image: meta.image.url,
    imageAlt: meta.image.alt,
  }}
/>
<div class="about-container">
  <div class="about-content">
    <h1 class="about-title">About</h1>
    <p class="about-text">
    I'm a university student at the University of
      <a
        href="https://www.tcu.ac.jp/english/"
        target="_blank"
        rel="noopener"
        class="about-link"
      >
        Tokyo City University
      </a>
      and a research assistant at
      <a
        href="https://www.jamstec.go.jp/e/"
        target="_blank"
        rel="noopener"
        class="about-link"
      >
        Japan Agency for Marine-Earth Science and Technology
      </a>
      .
    </p>
    <p class="about-text">
      I'm interested in automatic composition of music using deep learning .
      <br />
      Also, I'm interested in web development and I'm currently learning Svelte and FastAPI .
    </p>

    <h2 class="about-title">Links</h2>
      <ul class="about-list">
        <li>
          <a
            href="https://twitter.com/fightingsou"
            target="_blank"
            rel="noopener"
            class="about-link"
          >
            Twitter
          </a>
        </li>
        <li>
          <a
            href="https://github.com/fightingsou"
            target="_blank"
            rel="noopener"
            class="about-link"
          >
            GitHub
          </a>
        </li>
        <li>
          <a
            href="https://www.linkedin.com/in/hirawataso/"
            target="_blank"
            rel="noopener"
            class="about-link"
          >
            LinkedIn
          </a>
        </li>
        <li>
          <a
            href="https://www.instagram.com/hirawataso/"
            target="_blank"
            rel="noopener"
            class="about-link"
          >
            Instagram
          </a>
        </li>
        <li>
          <a
            href="mailto:hirawataso@gmail.com"
            target="_blank"
            rel="noopener"
            class="about-link"
          >
            Email
          </a>
        </li>
      </ul>
      <Awards />
      <Papers />
  </div>
</div>

<style>
  .about-container {
    display: flex;
    justify-content: center;
    align-items: center;
    font-family: georgia, serif;
    height: 100%;
    width: 100%;
  }

  .about-content {
    width: 100%;
    max-width: 800px;
    padding: 0 20px;
  }

  .about-title {
    font-size: 1.5rem;
    margin: 20px 0;
  }

  .about-list {
    list-style: none;
    padding: 0;
  }

  li {
    margin-left: 5px;
  }

  .about-text {
    margin: 10px 0;
  }

  .about-link {
    color: #0070f3;
    text-decoration: none;
  }
</style>
