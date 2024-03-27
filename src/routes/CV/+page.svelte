<script>
	import Tile from '../Tile.svelte';
	import { publications } from '../publications.js';

	const education = [
    "2011-2014 PhD thesis in molecular modelling, Université Paris Diderot-Paris 7, Paris, France",
    "2009-2011 Master in bioinformatics, Université Paris Diderot-Paris 7, Paris, France",
    "2008-2009 Exchange student at San José State University, San José, California, USA",
    "2005-2009 Bachelor in chemistry and biology, Université Paris 12, Créteil, France",
	];
	const positions = [
    "2018-2022 Postdoc in the Topf and Thalassinos groups , Birkbeck & UCL, University of London, London",
    "2014-2016 Wales group , University of Cambridge, Cambridge"
	];
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
			{publication.authors}, "{publication.Title}"
			<a href="http://doi.org/{publication.DOI}">doi: {publication.DOI}</a>
		</li>
	{/each}
</ul>

<h3>Positions</h3>
<ul>
	{#each positions as pos}
		<li>
			{pos}
		</li>
	{/each}
</ul>

<h3>Education</h3>
<ul>
	{#each education as edu}
		<li>
			{edu}
		</li>
	{/each}
</ul>

</main>
