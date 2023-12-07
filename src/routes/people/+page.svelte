<script>
	const lab_members = [
		"Gemma White",
		"Alison Faid",
		"Arek Wylegalski",
		"Anuregah Erlaut",
	];

	const collaborators = [
		"Konstantinos Thalassinos",
	];
</script>

<main>
<h1>Members of the lab</h1>

<ul>
	{#each lab_members as lab_member}
		<li>
			{lab_member}
		</li>
	{/each}
</ul>

<h1> Collaborators</h1>

<ul>
	{#each collaborators as colab}
		<li>
			{colab}
		</li>
	{/each}
</ul>

<h1>Previous Members</h1>

<ul>
	<li>
		Neil Anthony Magno
	</li>
</ul>


</main>
