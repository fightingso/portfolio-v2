<script lang="ts">
  export let post: Post;
  import { format } from "fecha";
</script>

<div class="post-item">
  <p class="post-item__date">{format(new Date(post.date), "MMMM DD, YYYY")}</p>
  <p class="post-item__title">
    <a class="post-item__title__link" href={`/blog/${post.slug}`}
      >{post.title}</a
    >
  </p>
  <p class="post-item__description">{post.description}</p>
</div>

<style>
  .post-item {
    border-bottom: solid 0.5px #999;
    padding: 1.4rem 0;
    margin-bottom: 1rem;
    line-height: 1.6;
  }
  .post-item__date {
    font-family: cursive;
    color: var(--secondary-color);
  }

  .post-item__title {
    font-size: 1rem;
    font-family: georgia, serif;
    margin: 0.5rem 0;
  }

  .post-item__title__link {
    color: var(--main-color);
    font-size: 1.5rem;
    text-decoration: none;
  }

  .post-item__description {
    font-family: georgia, serif;
    color: #444;
  }
</style>
