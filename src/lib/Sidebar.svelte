<script lang="ts">
	import Logo from './Logo.svelte';
	import NavBar from './NavBar.svelte';
</script>

<div>
	<Logo />
	<NavBar />
</div>

<style>
	div {
		width: fit-content;
		display: flex;
		flex-direction: column;
		gap: var(--margin-xl);
	}
</style>
