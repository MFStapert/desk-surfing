<script>
	import NavigationItem from './NavigationItem.svelte';

	import { Globe, Home, User } from 'svelte-hero-icons';
	let navItems = [
		{ label: 'Host', link: 'host', icon: Home },
		{ label: 'Work', link: 'work', icon: Globe },
		{ label: 'Profile', link: 'profile', icon: User },
	];
</script>

<nav class="flex flex-row justify-center md:flex-col my-4">
	{#each navItems as navItem}
		<NavigationItem {navItem} />
	{/each}
</nav>
