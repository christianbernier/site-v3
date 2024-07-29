<script lang="ts">
	import { page } from '$app/stores';

	export let label: string;
	export let path: string;

	$: isActive = () => $page.url.pathname === path;
</script>

<a href={path} style={`text-decoration: ${isActive() ? 'underline' : 'none'}`}>
	{label}
</a>

<style>
	a {
		font-size: var(--font-size-nav-link);
		font-weight: bold;
		letter-spacing: -1px;
	}
</style>
