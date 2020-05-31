<script>
  import Code from  '../../Code.svelte';
</script>

<h4 class="ct-preview-header">Preview</h4>

<div class="ct-preview">
 <div class="c-card">
     <p>Content</p>
  </div>
</div>

<Code>
  <div slot="html">
    <textarea class="ct-textarea ct-textarea--code textarea--code-full-component">{`<div class="c-card">
 <p>Content</p>
</div>`}</textarea>
  </div>
  <div slot="css">
    <textarea class="ct-textarea ct-textarea--code textarea--code-full-component">{`/* Card 
   ========================================================================== */

.c-card {
  background: $color-gray-200;
  border: 0.1rem solid $color-gray-200;
  border-radius: 0.3rem;
  padding: 1.6rem;
  margin: 0 0 1.6rem;
}
`}</textarea>
  </div>
</Code>
