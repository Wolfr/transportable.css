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


<div class="c-columns">
  <div class="c-columns__column">
      <h4>HTML</h4>
      <slot name="html"></slot>
  </div>
  <div class="c-columns__column">
      <h4>CSS</h4>
      <slot name="css"></slot>
  </div>
</div>
