<svelte:head>
  <link rel='stylesheet' href='/normalize.css'>
  <link rel='stylesheet' href='/build/global-css-vars.css'>
  <link rel='stylesheet' href='/build/transportable-docs.css'>
</svelte:head>

<style>
  .ct-textarea {
    height: 10rem;
    min-height: auto;
  }
</style>

<p>Medium paragraph</p>
<textarea class="ct-textarea ct-textarea--code textarea--code-full-component">{`
  <p>Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae, ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam egestas semper. Aenean ultricies mi vitae est. Mauris placerat eleifend leo.</p>
`}</textarea>

<p>Short paragraph</p>
<textarea class="ct-textarea ct-textarea--code textarea--code-full-component">{`
  <p>Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas.</p>
`}</textarea>

<p>Unordered list</p>
<textarea class="ct-textarea ct-textarea--code textarea--code-full-component">{`
  <ul>
     <li>Lorem ipsum dolor sit amet, consectetuer adipiscing elit.</li>
     <li>Aliquam tincidunt mauris eu risus.</li>
     <li>Vestibulum auctor dapibus neque.</li>
  </ul>
`}</textarea>

<p>Ordered list</p>
<textarea class="ct-textarea ct-textarea--code textarea--code-full-component">{`
  <ol>
     <li>Lorem ipsum dolor sit amet, consectetuer adipiscing elit.</li>
     <li>Aliquam tincidunt mauris eu risus.</li>
     <li>Vestibulum auctor dapibus neque.</li>
  </ol>
`}</textarea>



