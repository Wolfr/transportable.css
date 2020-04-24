<script>
  import Code from  './Code.svelte';
</script>
  
<style>
  /* Buttons
     ========================================================================== */

  :root {
    --button-default-bg: var(--gray-200);
    --button-default-color: var(--gray-700);
    --button-primary-bg: var(--blue-500);
    --button-primary-color: #FFF;
  }

  @media (prefers-color-scheme: dark) {
    :root {
      --button-default-bg: var(--gray-800);
      --button-default-color: var(--gray-300);
      --button-primary-bg: var(--blue-500);
    }
  }

  .c-button {
    padding: 0.8rem 1.4rem;
    display: inline-block;
    appearance: none;
    border-radius: 0.3rem;
    text-decoration: none;
  }

  .c-button--default {
    color: var(--button-default-color);
    background: var(--button-default-bg);
  }

  .c-button--primary {
    color: var(--button-primary-color);
    background: var(--button-primary-bg);
  }

</style>

<h4>Preview</h4>

<div class="c-preview">
  <a class="c-button c-button--default" href="/">Button</a>
  <a class="c-button c-button--primary" href="/">Button</a>
</div>

<Code>
  <div slot="html">
    <textarea class="c-textarea c-textarea--code">{`
  <a class="c-button c-button--default" href="/">Button</a>
  <a class="c-button c-button--primary" href="/">Button</a>
    `}</textarea>
  </div>
  <div slot="css">
    <textarea class="c-textarea c-textarea--code">{`
/* Buttons
   ======================================= */

:root {
  --button-default-bg: var(--gray-400);
  --button-default-color: var(--gray-700);
  --button-primary-bg: var(--blue-500);
  --button-primary-color: #FFF;
}

@media (prefers-color-scheme: dark) {
  :root {
    --button-default-bg: var(--gray-800);
    --button-default-color: var(--gray-300);
    --button-primary-bg: var(--blue-500);
  }
}

.c-button {
  padding: 0.8rem 1.4rem;
  display: inline-block;
  appearance: none;
  border-radius: 0.3rem;
  text-decoration: none;
}

.c-button--default {
  color: var(--button-default-color);
  background: var(--button-default-bg);
}

.c-button--primary {
  color: var(--button-primary-color);
  background: var(--button-primary-bg);
}
`}</textarea>
  </div>
</Code>


