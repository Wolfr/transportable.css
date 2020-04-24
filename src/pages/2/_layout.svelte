<style>

  .main-container {
    display: flex;
  }

  .main-container main {
    flex: 1 1 auto;
  }
  
  .main-container aside {
    flex: 0 0 24rem;
    margin-right: 2.4rem;
  }

</style>

<svelte:head>
  <link rel='stylesheet' href='/reset.css'>
  <link rel='stylesheet' href='/global-css-vars.css'>
</svelte:head>


<div class="main-container">
  <aside>

    <h4>1. Start here...</h4>

    <p>Copy this in your style sheet:</p>

    <ul>
      <li><a href="/2/reset">Reset</a></li>
    </ul>

    <h4>2. Now choose a color theme:</h4>

    <ul>
      <li><a href="/2/base-theme">Base theme</a></li>
    </ul>

    <h4>3. Now let's use some components</h4>

    <ul>
      <li><a href="/2/card">Card</a></li>
      <li><a href="/2/button">Button</a></li>
      <li><a href="/2/list">List</a></li>
    </ul>
  </aside>

  <main>
    <slot />
  </main>
</div>