<script>
  import { isActive, url } from '@sveltech/routify'

  export let no
</script>
  
<style>

  .active {
    font-weight: bold;
  }

  h4 {
    font-weight: 700;
    color: #000;
    padding: 0;
    margin: 0 0 1.2rem;
  }

  a {
    text-decoration: none;
    display: inline-block;
    padding: 0.6rem;
  }
  
  ul {
    list-style: none;
    padding: 0;
    margin: 0 0 1.2rem;
  }

  li {
    border-bottom: 0.1rem solid #CCC;
  }

  li:last-child {
    border: none;
  }

</style>

<h4>Pick CSS style</h4>
<ul>
  <li><a class:active={$isActive('/1')} href="/1">normalize.css + CSS variables</a></li>
  <li><a class:active={$isActive('/2')} href="/2">Reset + CSS variables</a></li>
  <li><a class:active={$isActive('/3')} href="/3">Reset + SCSS</a></li>
</ul>

<h4>1. Start here...</h4>

<p>Copy this in your style sheet:</p>

{#if no == 1}
<ul>
  <li><a href="/{no}/normalize">Normalize</a></li>
</ul>
{:else}
<ul>
  <li><a href="/{no}/reset">Reset</a></li>
</ul>
{/if}

<h4>2. Now choose a color theme:</h4>

<ul>
  <li><a href="/{no}/base-theme">Base theme</a></li>
</ul>

<h4>3. Now let's use some components</h4>

<ul>
  <li><a href="/{no}/components/card">Card</a></li>
  <li><a href="/{no}/components/button">Button</a></li>
  <li><a href="/{no}/components/desktop-list">Desktop - List</a></li>
  <li><a href="/{no}/components/badge">Badge</a></li>
  <li><a href="/{no}/components/avatar">Avatar</a></li>
  <li><a href="/{no}/components/table-view">Table view (mobile)</a></li>
</ul>
