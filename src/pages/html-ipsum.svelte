<svelte:head>
  <link rel='stylesheet' href='/normalize.css'>
  <link rel='stylesheet' href='/build/global-css-vars.css'>
</svelte:head>

<style>
  .c-textarea {
    height: 10rem;
    min-height: auto;
  }
</style>

<p>Medium paragraph</p>
<textarea class="c-textarea c-textarea--code">{`
  <p>Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae, ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam egestas semper. Aenean ultricies mi vitae est. Mauris placerat eleifend leo.</p>
`}</textarea>

<p>Short paragraph</p>
<textarea class="c-textarea c-textarea--code">{`
  <p>Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas.</p>
`}</textarea>

<p>Unordered list</p>
<textarea class="c-textarea c-textarea--code">{`
  <ul>
     <li>Lorem ipsum dolor sit amet, consectetuer adipiscing elit.</li>
     <li>Aliquam tincidunt mauris eu risus.</li>
     <li>Vestibulum auctor dapibus neque.</li>
  </ul>
`}</textarea>

<p>Ordered list</p>
<textarea class="c-textarea c-textarea--code">{`
  <ol>
     <li>Lorem ipsum dolor sit amet, consectetuer adipiscing elit.</li>
     <li>Aliquam tincidunt mauris eu risus.</li>
     <li>Vestibulum auctor dapibus neque.</li>
  </ol>
`}</textarea>



