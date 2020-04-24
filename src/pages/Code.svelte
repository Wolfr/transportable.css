<script>
  export let scss;
</script>
<style>

  h4 {
    font-size: 1.4rem;
    font-weight: 500;
    padding: 0 0 .4rem;
  }

  .c-columns {
    margin-top: 1.6rem;
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
