<nav class="header">
  <ul class="header__links">
    <li class="header__title">
      <a href="/" class="header__title__link">
        SO Hirawata
      </a>
    </li>
    <li class="header__links_item">
      <a href="/" class="header__links__item__link">Home</a>
    </li>
    <li class="header__links_item">
      <a href="/about" class="header__links__item__link">About</a>
    </li>
    <li class="header__links_item">
      <a href="mailto:hirawataso@gmail.com" class="header__links__item__link">
        Contact
      </a>
    </li>
  </ul>
</nav>

<style>
  .header {
    margin-top: 5rem;
    margin-bottom: 2rem;
    height: 6rem;
    display: flex;
    justify-content: space-between;
    flex-direction: row;
  }

  .header__links {
    display: flex;
    flex-direction: row;
    align-items: center;
    list-style: none;
  }

  .header__title {
    margin-right: 10rem;
    margin-left: 1rem;
    color: #111;
  }

  .header__title__link {
    font-size: 3rem;
    font-family: cursive;
    text-decoration: none;
    color: #333;
  }

  .header__links_item {
    font-family: cursive;
    margin-top: 2.2rem;
    margin-left: 2rem;
  }

  .header__links_item:last-child {
    margin-right: 1rem;
  }

  .header__links__item__link {
    color: var(--secondary-color);
    text-decoration: none;
  }

  .header__links__item__link:hover {
    border-bottom: 1.5px solid #ccc;
  }
</style>
