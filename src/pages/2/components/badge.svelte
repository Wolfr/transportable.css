<script>
  import Code from  '../../Code.svelte';
</script>

<h4 class="ct-preview-header">Preview</h4>

<div class="ct-preview">
  <div class="c-badge">Badge text</div>
</div>

<Code>
  <div slot="html">
    <textarea class="ct-textarea ct-textarea--code textarea--code-full-component">{`
<div class="c-badge">Badge text</div>
    `}</textarea>
  </div>
  <div slot="css">
    <textarea class="ct-textarea ct-textarea--code textarea--code-full-component">{`/* Badge
   ========================================================================== */

.c-badge {
  background: #DDD;
  color: #000;
  display: inline-block;
  border-radius: 1.2rem;
  padding: 0.3rem 1.2rem;
  font-size: 1.3rem;
}`}</textarea>
  </div>
</Code>


