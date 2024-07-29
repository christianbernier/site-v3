<script lang="ts">
	import { afterNavigate } from '$app/navigation';
	import Sidebar from '$lib/Sidebar.svelte';

	afterNavigate(() => {
		const content: HTMLDivElement | null = document.querySelector('#layout__content');
		if (content) {
			content.scrollTo({ top: 0 });
		}
	});
</script>

<div id="layout__container">
	<div id="layout__sidebar">
		<Sidebar />
	</div>
	<div id="layout__content">
		<slot></slot>
	</div>
</div>

<style>
	#layout__container {
		height: 100vh;
		display: grid;
		grid-template-columns: 2fr 3fr;
		grid-template-rows: auto;
	}

	#layout__sidebar {
		padding: var(--margin-top);
		background-color: var(--primary);
		display: flex;
		justify-content: flex-end;
	}

	#layout__content {
		padding: var(--margin-top);
		max-width: 80ch;
		overflow-y: auto;
		-ms-overflow-style: none;
		scrollbar-width: none;
	}

	#layout__content::-webkit-scrollbar {
		display: none;
	}

	@media only screen and (max-width: 850px) {
		#layout__container {
			height: fit-content;
			width: 100vw;
			grid-template-columns: auto;
			grid-template-rows: auto auto;
		}

		#layout__sidebar {
			padding: calc(2 * var(--margin-top)) var(--margin-top);
			justify-content: flex-start;
		}

		#layout__content {
			padding: calc(2 * var(--margin-top)) var(--margin-top);
			overflow-y: hidden;
		}
	}
</style>
