<script lang="ts">
	export let imageSource: string;
	export let name: string;
	export let location: string;
	export let datesAttended: string;
	export let subtitle: string;
	export let degree: string;
</script>

<div class="school__container">
	<img src={imageSource} alt={`${name} logo`} />
	<div class="school__text">
		<div>
			<p><span class="school__name">{name}</span>, {location}</p>
			<p class="school__subtitle">{subtitle}</p>
		</div>
		<div>
			<p>{degree}</p>
			<p>{datesAttended}</p>
		</div>
	</div>
</div>

<style>
	.school__container {
		display: flex;
		flex-direction: row;
		gap: 20px;
		margin-bottom: 20px;
	}

	img {
		width: 150px;
		height: 150px;
	}

	p {
		padding: 5px 0;
	}

	.school__text {
		display: flex;
		flex-direction: column;
		justify-content: space-between;
	}

	.school__name {
		font-weight: bold;
		font-size: 1.4rem;
	}

	.school__subtitle {
		font-weight: 300;
		padding: 0;
	}

	@media only screen and (max-width: 850px) {
		.school__container {
			flex-direction: column;
		}
	}
</style>
