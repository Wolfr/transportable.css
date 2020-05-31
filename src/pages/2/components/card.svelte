<script>
  import Code from  '../../Code.svelte';
</script>

<style>
  /* Card 
     ========================================================================== */

  .c-card  {
    --card-bg: var(--gray-100);
    --card-border: var(--gray-200);
  }

  @media (prefers-color-scheme: dark) {
    .c-card {
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

</style>

<h4 class="ct-preview-header">Preview</h4>

<div class="ct-preview">
 <div class="c-card">
     <p>Content</p>
  </div>
</div>

<Code>
  <div slot="html">
    <textarea class="ct-textarea ct-textarea--code textarea--code-full-component">{`
<div class="c-card">
 <p>Content</p>
</div>
    `}</textarea>
  </div>
  <div slot="css">
    <textarea class="ct-textarea ct-textarea--code textarea--code-full-component">{`
/* Card 
   ========================================================================== */

:root {
  --card-bg: var(--gray-100);
  --card-border: var(--gray-200);
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
