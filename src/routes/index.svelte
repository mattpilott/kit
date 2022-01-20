<script context="module">
   export async function load({ fetch, url }) {
      const res = await fetch(`/api.json`)

      if ( res.ok ) return { props: await res.json() }
   }
</script>

<script>
   export let success = false
</script>
{success}
<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
