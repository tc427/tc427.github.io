<script>
	import Tile from '../Tile.svelte';
</script>

<main>
<h1>My research</h1>

<div class="projects">
	<Tile
		title="Understand dynamic ensembles of biomolecular assemblies"
		summary="Use methods that inherently represent ensembles of models. Use them to understand molecular flexibility and dynamics."
	/>
	<Tile
		title="Cellular-scale molecular dynamics"
		summary="Develop novel methods to tackle large assemblies. Automated, scaling up of simulations to the meso-scale."
	/>
	<Tile
		title="Integrated biophysical modelling: end-to-end representations"
		summary="Integrate representation of biophysical experiment in data modelling."
	/>
</div>

</main>

<style>
.projects {
	display: grid;
	grid-template-columns: repeat(auto-fill, minmax(600px, 1fr));
	gap: 32px;
}
</style>
