<script lang="ts">
	import { Icon, Globe, Home, User } from 'svelte-hero-icons';
</script>

<nav class="my-4">
	<span
		class="side-nav-item active:font-normal  hover:bg-gray-100 px-6 font-semibold text-md cursor-pointer"
	>
		<Icon solid src={Home} class="h-8 w-8 mr-4 blue-300 text-blue-500 hover:text-blue-600  " />
		Host
	</span>
	<span
		class="side-nav-item active:font-normal  hover:bg-gray-100 px-6 font-semibold text-md cursor-pointer"
	>
		<Icon solid src={Globe} class="h-8 w-8 mr-4 blue-300 text-blue-500 hover:text-blue-600  " />
		Visit</span
	>
	<span
		class="side-nav-item active:font-normal  hover:bg-gray-100 px-6 font-semibold text-md cursor-pointer"
	>
		<Icon solid src={User} class="h-8 w-8 mr-4 blue-300 text-blue-500 hover:text-blue-600  " />
		Profile</span
	>
</nav>

<!-- {/each} -->
<style>
	.side-nav-item {
		@apply flex items-center
		text-sm py-3 px-8 rounded
		transition duration-300 ease-in-out;
	}
</style>
