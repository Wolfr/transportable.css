<script>
  import SidebarContent from '../SidebarContent.svelte';
</script>

<svelte:head>
  <link rel='stylesheet' href='/normalize.css'>
  <link rel='stylesheet' href='/build/global-css-vars.css'>
  <link rel='stylesheet' href='/build/transportable-docs.css'>
</svelte:head>

<div class="ct-main-container">
  <aside>
    <SidebarContent no="1" />
  </aside>
  <main>
    <slot />
  </main>
</div>