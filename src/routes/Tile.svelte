<script>
	import github from '$lib/images/github.svg';
	import link_img from '$lib/images/link.svg';

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
			<img src={link_img} alt="link to project" height="20vh" />
		</a>
		{/if}
		{#if source != ""}
		<a href={source}>
			<img src={github} alt="GitHub" height="20vh" />
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
</style>
