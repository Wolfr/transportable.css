<script>
  import Code from  '../../Code.svelte';
</script>
  
<style>

  /* Avatar
     ========================================================================== */

  .c-avatar {
    width: 3.2rem;
    height: 3.2rem;
    line-height: 3.2rem;
    text-align: center;
    font-size: 1.6rem;
    border-radius: 100%;
    background: #DDD;
  }

</style>

<h4 class="ct-preview-header">Preview</h4>

<div class="ct-preview">
  <div class="c-avatar">JR</div>
</div>

<Code>
  <div slot="html">
    <textarea class="ct-textarea ct-textarea--code textarea--code-full-component">{`
<div class="c-avatar">JR</div>
    `}</textarea>
  </div>
  <div slot="css">
    <textarea class="ct-textarea ct-textarea--code textarea--code-full-component">{`/* Avatar
   ========================================================================== */

.c-avatar {
  width: 3.2rem;
  height: 3.2rem;
  line-height: 3.2rem;
  text-align: center;
  font-size: 1.6rem;
  border-radius: 100%;
  background: #DDD;
}
`}</textarea>
  </div>
</Code>


