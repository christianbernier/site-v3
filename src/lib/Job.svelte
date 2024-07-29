<script lang="ts">
	export let imageSource: string;
	export let companyName: string;
	export let positionTitle: string;
	export let dates: string;
	export let location: string;
	export let description: string;
	export let responsibilities: string[];
</script>

<div class="job__container">
	<div class="job__summary">
		<img src={imageSource} alt={`${companyName} logo`} />
		<div class="job__header">
			<div>
				<p class="job__company-name">{companyName}</p>
				<p class="job__position-title">{positionTitle}</p>
			</div>
			<div class="job__secondary-information">
				<p>{dates}</p>
				<p>{location}</p>
			</div>
		</div>
	</div>

	<p>{description}</p>
	<ul>
		{#each responsibilities as responsibility}
			<li>{responsibility}</li>
		{/each}
	</ul>
</div>

<style>
	.job__container {
		margin-bottom: 50px;
	}

	.job__summary {
		display: flex;
		flex-direction: row;
		gap: 20px;
		margin-bottom: 20px;
	}

	img {
		width: 120px;
		height: 120px;
		border-radius: 6px;
	}

	p {
		padding: 5px 0;
	}

	ul {
		list-style-type: square;
	}

	.job__header {
		display: flex;
		flex-direction: column;
		justify-content: space-between;
	}

	.job__company-name {
		font-weight: bold;
		font-size: 1.4rem;
	}

	.job__position-title {
		font-style: italic;
		padding: 0;
	}

	.job__secondary-information p {
		font-size: 1rem;
		font-weight: 300;
		padding: 2px 0;
	}

	@media only screen and (max-width: 850px) {
		.job__summary {
			flex-direction: column;
		}
	}
</style>
