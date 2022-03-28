<script>
	import NavigationItem from './NavigationItem.svelte';

	import { Globe, Home, User } from 'svelte-hero-icons';
	let navItems = [
		{ label: 'Host', icon: Home },
		{ label: 'Work', icon: Globe },
		{ label: 'Profile', icon: User },
	];
</script>

<nav class="flex flex-row justify-center md:flex-col my-4">
	{#each navItems as navItem}
		<NavigationItem {navItem} />
	{/each}
</nav>
