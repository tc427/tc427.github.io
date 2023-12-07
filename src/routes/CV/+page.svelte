<script>
	import Tile from '../Tile.svelte';
	import { publications } from '../publications.js';
</script>

<main>

<h1>
	Tristan Cragnolini
</h1>

<h2>
	Lecturer
</h2>
<h3>
	Birbeck, University of London
</h3>

<h3>Publications</h3>
<ul>
	{#each publications as publication}
		<li>
			{publication.Title}
			doi: {publication.DOI}
		</li>
	{/each}
</ul>


</main>
