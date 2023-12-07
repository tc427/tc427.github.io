<script>
	import github from '$lib/images/github.svg';
	import link_img from '$lib/images/link.svg';

	export let title = "Title";
	export let authors = "";
	export let summary = "A short summary of this tile.";
	export let link = "";
	export let publication = "";
</script>

<section class="tile">
	<header>
		<h1>
			{title}
		</h1>
		<p>{authors}</p>
	</header>

	<details>
		<summary>Read more...</summary>
		<p>{summary}</p>
	</details>

	<footer>
		{#if link != ""}
		<a href={link}>
			<img src={github} alt="GitHub" height="20vh" />
		</a>
		{/if}
		{#if publication != ""}
		<a href={publication}>
			paper
			<img src={link_img} alt="publication link" height="20vh" />
		</a>
		{/if}
	</footer>
</section>

<style>
.tile {
	background-color: rgba(0, 0, 0, 0.1);
	padding: 32px;
	border-radius: 8px;
}
.tile header {
	display: inline;
}
footer {
	margin: 8px;
}
</style>
