<script>
  export let scss;
</script>
<style>
  
  .c-columns {
    display: flex;
    width: 100%;
  }
  
  .c-columns__column {
    flex: 1 1 auto;
  }
  
  .c-columns__column:first-child {
    margin-right: 1.6rem;
  }

  .c-columns__column:last-child {
    margin-left: 1.6rem;
  }

</style>
{scss}

<div class="c-columns">
  <div class="c-columns__column">
      <h4>HTML</h4>
      <slot name="html"></slot>
  </div>
  <div class="c-columns__column">
      {#if scss}
        <h4>SCSS</h4>
      {:else}
        <h4>CSS</h4>
      {/if}
      <slot name="css"></slot>
  </div>
</div>
