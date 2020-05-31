<script>
  import Code from  '../../Code.svelte';
</script>

<h4 class="ct-preview-header">Preview</h4>

<div class="ct-preview">
  <a class="c-button c-button--default" href="/">Button</a>
  <a class="c-button c-button--primary" href="/">Button</a>
</div>

<Code>
  <div slot="html">
    <textarea class="ct-textarea ct-textarea--code textarea--code-full-component">{`<a class="c-button c-button--default" href="/">Button</a>
<a class="c-button c-button--primary" href="/">Button</a>`}</textarea>
  </div>
  <div slot="css">
    <textarea class="ct-textarea ct-textarea--code textarea--code-full-component">{`/* Buttons
   ========================================================================== */

.c-button {
  padding: 0.8rem 1.4rem;
  display: inline-block;
  appearance: none;
  border-radius: 0.3rem;
  text-decoration: none;
}

.c-button--default {
  &,
  &:link,
  &:visited {
    color: $color-gray-500;
    background: $color-gray-100;
  }
}

.c-button--primary {
  &,
  &:link,
  &:visited {
    color: #FFF;
    background: $color-blue-500;
  }
}
`}</textarea>
  </div>
</Code>


