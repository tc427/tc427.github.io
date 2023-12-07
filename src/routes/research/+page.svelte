<script>
	import Tile from '../Tile.svelte';
</script>

<main>
<h1>My research</h1>

<div class="projects">
	<Tile
		title="Contact prediction with deep learning in flexible proteins"
		summary="We build models to predict contact between distant sites in proteins."
	/>
	<Tile
		title="Hierarchical coarse-grain modelling"
		summary="we investigate how coarse-grain mappings at different resolutions relate to one another and run simulations on biomolecular systems using those simplified models."
	/>
	<Tile
		title="Conformational sampling of protein structure prediction"
		summary="We develop statistical models to improve the sampling of alternative conformational states in protein structure prediction pipelines."
	/>
	<Tile
		title="Flexible fitting for cryo-EM"
		summary="We develop statistical models to represent the relation between structural variations in biomolecular complexes and the observed cryo-EM density."
	/>
</div>

</main>

<style>
.projects {
	display: grid;
	grid-template-columns: repeat(auto-fill, minmax(400px, 1fr));
	gap: 32px;
}
</style>
