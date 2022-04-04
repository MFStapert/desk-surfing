<script lang="ts">
	export let title = null;
</script>

<div class="h-min min-w-fit m-2 rounded bg-white shadow-sm">
	{#if title}
		<div class="p-4 border-b-2 border-slate-50">
			<h2 class="text-2xl font-semibold">{title}</h2>
		</div>
	{/if}

	<div class="p-4 w-full">
		<slot />
	</div>
	{#if $$slots.controls}
		<div class="flex flex-row-reverse p-4 border-t-2 border-slate-50">
			<slot name="controls" />
		</div>
	{/if}
</div>
