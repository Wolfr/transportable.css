<script>
  import Code from  '../Code.svelte';
  
  const items = [
    {
      id: 1,
      company: 'Mono',
      jobTitle: 'User interface designer',
      text: '<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>',
      linkUrl: 'https://mono.company/jobs/ui-designer-developer-apprenticeship/',
      imageUrl: 'http://placehold.it/200x150',
    },
    {
      id: 2,
      company: 'Mono',
      jobTitle: 'User interface designer',
      text: '<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>',
      linkUrl: 'https://mono.company/jobs/ui-designer-developer-apprenticeship/',
      imageUrl: 'http://placehold.it/200x150',
    }
  ]

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

  /* List
     ======================================= */

  :root {
    --list-border: var(--gray-300);
  }

  @media (prefers-color-scheme: dark) {
    :root {
      --list-border: var(--gray-700);
    }
  }

  .c-list {
    list-style: none;
    padding: 0;
  }

  .c-list li {
    border-bottom: 0.1rem solid var(--list-border);
    padding: 2.4rem;
  }

  .c-list li:last-child {
    border: none;
  }

  .c-list img {
    width: 10rem;
  }

  .c-list header h3 {
    margin: 0;
    padding: 0;
  }

  .c-list header {
    display: flex;
    align-items: center;
  }

  .c-list header .cover {
    flex: 0 0 auto;
    padding-right: 1.5rem;
  }

  .c-list header .inner {
    flex: 1 1 auto;
  }
</style>
<h4>Dependency</h4>

<ul>
  <li>Button</li>
</ul>

<h4 class="c-preview-header">Preview</h4>

<div class="c-preview">
  <ul class="c-list">
    {#each items as item}
      <li>
          <!-- <strong>{item.id}</strong> -->
          <header>
            <div class="cover">
              <img src="{item.imageUrl}" />
            </div>
            <div class="inner">
              <h3>{item.jobTitle}</h3>
              <p>{item.company}</p>
            </div>
          </header>
          <div class="c-content">
            {@html item.text}
          </div>
          <a class="c-button c-button--default" href={item.linkUrl}>View job post</a>
        </li>
    {/each}
  </ul>

</div>

<Code scss>
  <div slot="html">
    <textarea class="c-textarea c-textarea--code">{`
<ul class="c-list">
    <li>
        <header>
            <div class="cover "><img src="http://placehold.it/200x150"></div>
            <div class="inner ">
                <h3>User interface designer</h3>
                <p>Mono</p>
            </div>
        </header>
        <div class="c-content ">
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
        </div> <a class="c-button c-button--default " href="https://mono.company/jobs/ui-designer-developer-apprenticeship/">View job post</a> </li>
    <li>
        <header>
            <div class="cover "><img src="http://placehold.it/200x150"></div>
            <div class="inner ">
                <h3>User interface designer</h3>
                <p>Mono</p>
            </div>
        </header>
        <div class="c-content ">
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
        </div> <a class="c-button c-button--default " href="https://mono.company/jobs/ui-designer-developer-apprenticeship/">View job post</a> </li>
</ul>
    `}</textarea>
  </div>
  <div slot="css">
    <textarea class="c-textarea c-textarea--code">{`
/* List
   ========================================================================== */

.c-list {
  list-style: none;
  padding: 0;
}

.c-list li {
  border-bottom: 0.1rem solid $color-gray-300;
  padding: 2.4rem;
}

.c-list li:last-child {
  border: none;
}

.c-list img {
  width: 10rem;
}

.c-list header h3 {
  margin: 0;
  padding: 0;
}

.c-list header {
  display: flex;
  align-items: center;
}

.c-list header .cover {
  flex: 0 0 auto;
  padding-right: 1.5rem;
}

.c-list header .inner {
  flex: 1 1 auto;
}
`}</textarea>
  </div>
</Code>