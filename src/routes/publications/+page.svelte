<script>
	import Publication from './Publication.svelte';
	import { publications } from '../publications.js';
	import { browser as isThisaBrowser } from '$app/environment';
</script>

{#if isThisaBrowser}
<script async src="https://badge.dimensions.ai/badge.js" charset="utf-8"></script>
{/if}

<main>
<h1>Publications</h1>


<div class="projects">
	{#each publications as publication}
		<Publication
			title={publication.Title}
			authors={publication.authors}
			summary={publication["Abstract Note"]}
			publication={publication.Url}
			DOI={publication.DOI}
		/>
	{/each}
</div>

</main>

<style>
.projects {
	display: grid;
	grid-template-columns: repeat(auto-fill, minmax(600px, 1fr));
	gap: 32px;
}
</style>
