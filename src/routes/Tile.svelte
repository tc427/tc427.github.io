<script>
	import Github from './Github.svelte';
	import Link from './Link.svelte';

	export let title = "Title";
	export let summary = "A short summary of this tile.";
	export let link = "";
	export let source = "";
</script>

<section class="tile">
	<header>
		<h1>
			{title}
		</h1>
	</header>

	{summary}

	<footer>
		{#if link != ""}
		<a href={link}>
			<Link />
		</a>
		{/if}
		{#if source != ""}
		<a href={source}>
			<Github />
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
footer {
	margin: 8px;
}
.tile a {
	display: inline-block;
	min-height: 1em;
}
</style>
