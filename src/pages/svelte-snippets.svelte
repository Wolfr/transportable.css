<svelte:head>
  <link rel='stylesheet' href='/normalize.css'>
  <link rel='stylesheet' href='/build/global-css-vars.css'>
  <link rel='stylesheet' href='/build/transportable-docs.css'>
</svelte:head>

<p>Generate array</p>
<textarea class="ct-textarea ct-textarea--code" rows="5">{`
{#each {length: 20} as elem}
Oi
{/each}
`}</textarea>

<p>Push object into array (reactive)</p>
<textarea class="ct-textarea ct-textarea--code">{`
`}</textarea>


<p>View an object (with JSON stringify)</p>
<textarea class="ct-textarea ct-textarea--code" rows="25">{`
  <script>
  	let name = [
   {
     name: "Route",
     url: "/route/",
     routes: [
       {
         name: "Route subdir",
         url: "/route/subdir"
       },
       {
         name: "Route subdir 2",
         url: "/route/subdir2 "
       }
     ]
   }
  ]
  </script>

  <pre>
    {JSON.stringify(name, null, 2)}
  </pre>
`}</textarea>
