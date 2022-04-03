<script>
	export let photo;
	export let fullName;
	export let location;
</script>

<div class="flex flex-col min-w-fit m-2 p-4 rounded bg-white items-center space-x-4">
	<img
		src="{photo}.jpg"
		alt=""
		class="flex-none w-32 h-32 rounded-full object-cover"
		loading="lazy"
	/>

	<h2 class="text-2xl font-semibold">{fullName}</h2>
	<span class="text-blue-500 mt-0.5">{location}</span>
</div>
