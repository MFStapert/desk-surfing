<script lang="ts">
	import { Icon } from 'svelte-hero-icons';
	export let navItem;
</script>

<span
	class="side-nav-item active:font-normal  hover:bg-gray-100 px-6 font-semibold text-md cursor-pointer"
>
	<Icon
		solid
		src={navItem.icon}
		class="h-8 w-8 mr-4 blue-300 text-blue-500 hover:text-blue-600  "
	/>
	{navItem.label}
</span>

<!-- {/each} -->
<style>
	.side-nav-item {
		@apply flex items-center
		text-sm py-3 px-8 rounded
		transition duration-300 ease-in-out;
	}
</style>
