<script lang="ts">
	import { Icon } from 'svelte-hero-icons';
	export let navItem;
</script>

<a
	class="flex flex-col md:flex-row md:justify-start justify-center grow side-nav-item md:py-3 md:px-6 active:font-normal items-center hover:bg-gray-100 font-semibold text-md cursor-pointer"
	href={navItem.link}
>
	<Icon
		solid
		src={navItem.icon}
		class="hidden md:block md:mr-4 w-8 blue-300 text-blue-500 hover:text-blue-600  "
	/>
	{navItem.label}
</a>

<style>
	.side-nav-item {
		@apply text-sm rounded
		transition duration-300 ease-in-out;
	}
</style>
