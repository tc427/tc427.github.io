<script>
	import Tile from '../Tile.svelte';
</script>

<main>
<h1>My research</h1>

<div class="projects">
	<Tile
		title="Understand dynamic ensembles of biomolecular assemblies"
		summary=" To understand biomolecular assemblies, we need to represent the ensemble of conformations they go through to perform their function, from folding, to enzymatic mechanisms. This require methods that inherently represent these ensembles. I develop probabillistic models and methods, that can handle a distribution of conformations, and use them to understand molecular flexibility and dynamics."
		details={["Contact prediction with deep learning in flexible proteins",
			 "Conformational sampling of protein structure prediction"]}
	/>
	<Tile
		title="Cellular-scale molecular dynamics"
		summary="To understand the biophysics of cellular assemblies, new tools are required. I develop methods that automate the process of scaling up simulations, enabling the representations of process at the mesoscale."
		details={["Hierarchical coarse-grain modelling",
			 "Mycobacterium cell wall"]}
	/>
	<Tile
		title="Integrated biophysical modelling: end-to-end representations"
		summary="To interpret biophysical data, a detailed understanding of the process that produce this data is paramount. My work focus on developing end-to-end representations of biophysical experiments, to accurately understand the data they produce."
		details={["Flexible fitting for cryo-EM",
			 "Statistical interpretation of XL-MS data"]}
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
