<script>
	import { blur, fade, fly, slide } from 'svelte/transition';

	import github from '$lib/images/github.svg';
	import link_img from '$lib/images/link.svg';

	export let title = "Title";
	export let authors = "";
	export let summary = "A short summary of this tile.";
	export let link = "";
	export let publication = "";
	export let DOI = "";
	let open = false;
</script>

<section class="tile">
	<header>
		<h3>
			{title}
		</h3>
		<p>{authors}</p>
	</header>

	{#if summary}
	<details bind:open>
		<summary>Abstract</summary>
		{#if open}
			<p transition:slide={{ duration: 1000 }} >{summary}</p>
		{/if}
	</details>
	{/if}

	<footer>
		{#if DOI}
		<a href=https://doi.org/{DOI}>
			DOI: {DOI}
		</a>
		{/if}
		{#if link}
		<a href={link}>
			<img src={github} alt="GitHub" height="20vh" />
		</a>
		{/if}
		{#if publication}
		<a href={publication}>
			paper
			<img src={link_img} alt="publication link" height="20vh" />
		</a>
		{/if}
		{#if DOI}
			<span class="__dimensions_badge_embed__" data-doi="{DOI}" data-style="small_circle"></span>
		{/if}

	</footer>
</section>

<style>
details {
	margin: 20px;
	margin: 20px;
}
summary {
	color: var(--color-theme-1);
}
.tile {
	display: flex;
	flex-direction: column;
	justify-content: space-between;
	background-color: rgba(0, 0, 0, 0.1);
	padding: 0px 12px;
	margin: 12px;
	border-radius: 8px;
	position: relative;
}
.tile header {
	display: inline;
}
.tile footer {
	padding: 5px;
	margin: 5px;
}
footer {
	display: flex;
	flex-direction: row;
	justify-content: space-between;
}
footer a {
	margin: auto 8px;
}
.__dimensions_badge_embed__ {
	display: inline;
}
</style>
