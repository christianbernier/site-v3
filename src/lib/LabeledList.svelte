<script lang="ts">
	export let title: string;
	export let items: string[];
</script>

<div>
	<p>{title}</p>
	<ul>
		{#each items as item}
			<li>{item}</li>
		{/each}
	</ul>
</div>

<style>
	div {
		display: grid;
		grid-template-columns: 1fr 2fr;
		padding: 20px 0;
	}

	p {
		font-weight: bold;
	}

	p,
	li {
		padding: 0;
	}

	li + li {
		margin: 8px 0;
	}

	ul {
		margin: 0;
		list-style-type: none;
	}
</style>
