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
	<Tile
		title="HiRE-RNA coarse-grain model"
		summary="HiRE-RNA is a coarse grain nucleic acid forcefield, develop to accurately reproduce the interactions between nucleobases that drives nucleic acid folding. Work with Samuela Pasquali. Parametrisation with Yoann Laurin."
		publication="https://pubs.acs.org/doi/10.1021/jp400786b"
	/>
	<Tile
		title="Interpolation with Network Model"
		summary=" Interpolation with Network Model is a small program that computes an interpolation between two protein structures by moving along low-frequency normal modes computed on a structure, towards the final structure."
		source="https://github.com/tc427/inm"
	/>
	<Tile
		title="Webnm@"
		summary="Webnm@ is an online tool to compute, compare, and analyse normal modes for protein structures."
		link="http://apps.cbu.uib.no/webnma3"
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
