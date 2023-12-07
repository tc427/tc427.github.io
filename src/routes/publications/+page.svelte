<script>
	import Publication from './Publication.svelte';
</script>

<main>
<h1>Publications</h1>

<h2>2022</h2>

<div class="projects">
	<Publication
		title="Integrating simulation tools and Electron Microscopy"
		authors="Beton, Joseph; Cragnolini, Tristan; Kaleel, Manaz; Mulvaney, Thomas; Sweeney, Aaron; Topf, Maya;"
	/>
	<Publication
		title="Cryo-EM Structure and B-Factor Refinement with Ensemble Representation"
		authors="Cragnolini, T.; Beton, J.; Topf, M."
	/>
	<Publication
		title="Conformational sampling of protein structure prediction"
		summary="We develop statistical models to improve the sampling of alternative conformational states in protein structure prediction pipelines."
	/>
	<Publication
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
