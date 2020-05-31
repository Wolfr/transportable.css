<script>
  import SidebarContent from '../SidebarContent.svelte';
</script>
<style>

  .ct-main-container {
    display: flex;
  }

  .ct-main-container main {
    flex: 1 1 auto;
  }
  
  .ct-main-container aside {
    flex: 0 0 24rem;
    margin-right: 2.4rem;
  }

</style>

<svelte:head>
  <link rel='stylesheet' href='/reset.css'>
  <link rel='stylesheet' href='/build/scssversion.css'>
  <link rel='stylesheet' href='/build/transportable-docs.css'>
</svelte:head>

<div class="ct-main-container">
  <aside>
    <SidebarContent no="3" />
  </aside>
  <main>
    <slot />
  </main>
</div>