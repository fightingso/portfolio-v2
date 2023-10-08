<style>
  .container {
    position: fixed;
    bottom: 0;
    left: 0.2rem;
    z-index: 100;
    margin-bottom: 0.5rem;
  }

  .scrolldown {
    position: absolute;
    bottom: 10px;
    left: 50%;
  }

  .scrolldown span {
    position: absolute;
    left: 8px;
    bottom: 30px;
    color: #aaa;
    font-size: 0.8rem;
    letter-spacing: 0.05em;
    -ms-writing-mode: tb-rl;
    -webkit-writing-mode: vertical-rl;
    writing-mode: vertical-rl;
  }

  .scrolldown:before {
    content: "";
    position: absolute;
    bottom: 0;
    left: -4px;
    width: 10px;
    height: 10px;
    border-radius: 50%;
    background: #eee;
    animation:
      circlemove 1.6s ease-in-out infinite,
      cirlemovehide 1.6s ease-out infinite;
  }

  @keyframes circlemove{
    0%{bottom: 90px;}
    100%{bottom: -5px;}
  }

  @keyframes cirlemovehide{
    0%{opacity: 0;}
    50%{opacity: 1;}
    80%{opacity: 0.9;}
    100%{opacity: 0;}
  }

  .scrolldown:after{
    content: "";
    position: absolute;
    bottom: 0;
    left: 0;
    width: 2px;
    height: 100px;
    background: #aaa;
  }

  @media screen and (max-width: 768px) {
    .scrolldown {
      display: none;
    }
  }
</style>

<div class="container">
  <div class="scrolldown"><span>Scroll</span></div>
</div>
