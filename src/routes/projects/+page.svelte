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
		summary=" We investigate how coarse-grain mappings at different resolutions relate to one another and run simulations on biomolecular systems using those simplified models. We use graph representations and graph neural networks to automate the coarse-graining of proteins at varying levels of description and run molecular dynamics simulations using these simplified models with the aim of striking a balance between accuracy and computational cost."
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
		summary=" With my PhD supervisor Samuela Pasquali, we worked on developing the HiRE-RNA forcefield to represent complex interactions in RNA and DNA, and create a model that could truly represent the full range of possible RNA structures, without external constraints that do not correspond to a biophysical force. This 'bottom-up' approach could then be combined with experimental restraints, as obtainable from cryo-EM, SAXS, etc...  ."
		publication="https://pubs.acs.org/doi/10.1021/jp400786b"
	/>
	<Tile
		title="Protein and nucleic acid folding: disorder and ensembles"
		summary="Work on G-quadruplexes with David Wales, Debayan Chakraborty, Liuba Mazzanti, Jiří Šponer, Samuela Pasquali, Philippe Derreumaux. We obtained pathways between common states using MD and pathsampling. "
	/>
	<Tile
		title="Protein and nucleic acid folding: disorder and ensembles"
		summary="I have studied RNA, DNA and protein folding using different models. I have been particularly interested in metastable systems, such as riboswitches, G-quadruplexes, and co-folding proteins. I am keen on delving further into the assembly of larger biomolecular complexes. "
	/>
	<Tile
		title="SELEX analysis and simulation"
		summary="Trying to understand how SELEX works, what can we tell about the obtained sequence, the likeliness of them binding to the target.  Work with Lucy Colwell, Alaa Abdel-Latif, and Centauri (Helen Lavender, Alex Martin). "
		source="https://github.com/tc427/SELEX_Sim_v0.3"
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
