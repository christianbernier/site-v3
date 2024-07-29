<script lang="ts">
	export let title: string;
	export let link: string | undefined = undefined;
	export let dates: string;
	export let technologies: string;
	export let bullets: string[];
</script>

<div class="project__container">
	<p class="project__title">{title}</p>
	<div class="project__secondary-information">
		<p>
			{#if link}
				<a href={link}>View live</a>
				<span class="bullet">•</span>
			{/if}
			{dates}
			<span class="bullet">•</span>
			{technologies}
		</p>
	</div>
	<ul>
		{#each bullets as bullet}
			<li>{bullet}</li>
		{/each}
	</ul>
</div>

<style>
	.project__container {
		padding: 20px 0;
	}

	p {
		padding: 5px 0;
	}

	ul {
		list-style-type: square;
	}

	.project__title {
		font-weight: bold;
		font-size: 1.4rem;
	}

	.project__secondary-information p {
		font-size: 1rem;
		font-weight: 300;
		padding: 2px 0;
	}

	.bullet {
		font-size: 0.8rem;
		margin: 0 2px;
	}
</style>
