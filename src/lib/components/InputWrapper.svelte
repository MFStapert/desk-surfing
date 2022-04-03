<script lang="ts">
	export let title: string;
</script>

<div class="mb-2">
	<span class="block mb-2 text-gray-700">{title}</span>
	<slot />
</div>
