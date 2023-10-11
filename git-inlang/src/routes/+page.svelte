<script lang="ts">
  import {i, languages, switchLanguage} from '@inlang/sdk-js';
</script>


<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

{#each languages as lang} 
  <button on:click={() => switchLanguage(lang)}>{lang}</button>
{/each}

<h1>{i('message', {name: 'house'})}</h1>