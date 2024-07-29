<script lang="ts">
	import NavLink from './NavLink.svelte';
</script>

<nav>
	<NavLink label="about" path="/" />
	<NavLink label="education" path="/education" />
	<NavLink label="experience" path="/experience" />
	<NavLink label="projects" path="/projects" />
</nav>

<style>
	nav {
		width: fit-content;
		display: flex;
		flex-direction: column;
		gap: var(--nav-link-spacing);
	}
</style>
