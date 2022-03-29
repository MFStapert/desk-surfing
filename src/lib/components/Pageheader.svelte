<script>
	export let title;
</script>

<div class="bg-gray-100">
	<div class="w-4/6 mx-auto py-20">
		<h1 class="font-bold text-4xl mb-4">{title}</h1>
		<span class="text-gray-800 ">
			<slot />
		</span>
	</div>
</div>
