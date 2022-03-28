<script>
	import { Icon, SwitchHorizontal, Search } from 'svelte-hero-icons';
</script>

<div class="my-auto flex flex-row items-center">
	<div class="flex items-center w-48 cursor-pointer">
		<Icon
			solid
			src={SwitchHorizontal}
			class="h-8 w-8 mr-4 blue-300 text-blue-500 hover:text-blue-600 "
		/>
		<span class="font-semibold text-blue-500 hover:text-blue-600">Desksurfing</span>
	</div>

	<div class="flex align-baseline self-center p-1 border rounded-md border-gray-400">
		<Icon solid src={Search} class="h-6  w-6 mr-2  text-gray-400" />
		<input class="outline-none" placeholder="search" />
	</div>
</div>
