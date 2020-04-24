<script>
  import { isActive, url } from '@sveltech/routify'
</script>
<style>

  header {
    display: flex;
    justify-content: space-between;
    padding: 2.4rem 0;
  }

  .active {font-weight: bold}

  nav a {
    text-decoration: none;
    display: inline-block;
    margin-right: 2rem;
  }
  h2 {
    font-size: 2rem;
    margin: 0;
    padding: 0;
  }
  h2 a {
    text-decoration: none;
  }
</style>
<header>
  <h2><a href="/">Transportable.css</a></h2>
  <nav>
    <a class:active={$isActive('/1')} href="/1">normalize.css + CSS variables</a>
    <a class:active={$isActive('/2')} href="/2">Reset + CSS variables</a>
    <a class:active={$isActive('/3')} href="/3">Reset + SCSS</a>
  </nav>
</header>

<slot />
