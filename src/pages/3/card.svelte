<script>
  import Code from  './Code.svelte';
</script>

<style lang="scss">
  /* Card 
     ========================================================================== */

/*  $c-card-bg: $gray-200 !default;
  $c-card-border: $gray-100 !default;
*/

  .c-card {
/*    background: $c-card-bg;
    border: 0.1rem solid $c-card-border;*/
    border-radius: 0.3rem;
    padding: 1.6rem;
    margin: 0 0 1.6rem;
  }

</style>

<h4>Preview</h4>

<div class="c-preview">
 <div class="c-card">
     <p>Content</p>
  </div>
</div>

<Code>
  <div slot="html">
    <textarea class="c-textarea c-textarea--code">{`
<div class="c-card">
 <p>Content</p>
</div>
    `}</textarea>
  </div>
  <div slot="css">
    <textarea class="c-textarea c-textarea--code">{`
/* Card 
   ========================================================================== */

:root {
  --card-bg: var(--gray-200);
  --card-border: var(--gray-100);
}

@media (prefers-color-scheme: dark) {
  :root {
    --card-bg: var(--gray-900);
    --card-border: var(--gray-900);
  }
}

.c-card {
  background: var(--card-bg);
  border: 0.1rem solid var(--card-border);
  border-radius: 0.3rem;
  padding: 1.6rem;
  margin: 0 0 1.6rem;
}
    `}</textarea>
  </div>
</Code>
