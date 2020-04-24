<script>
  import SidebarContent from '../SidebarContent.svelte';
</script>

<svelte:head>
  <link rel='stylesheet' href='/normalize.css'>
  <link rel='stylesheet' href='/build/global-css-vars.css'>
</svelte:head>


<div class="main-container">
  <aside>
    <SidebarContent no="1" />
  </aside>

  <main>
    <slot />
  </main>
</div>