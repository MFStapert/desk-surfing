<script lang="ts">
	import Card from '$lib/components/Card.svelte';
</script>

<Card title="References">
	{#each ['Janet', 'Jane', 'Jacky', 'Joe'] as name}
		<a href="profile">
			<div class="flex flex-col md:flex-row p-4 border-b border-slate-200 hover:bg-gray-200">
				<img
					src="{name}.jpg"
					alt=""
					class="flex-none w-32 h-32 rounded-full object-cover mr-4"
					loading="lazy"
				/>
				<div class="flex flex-col w-full">
					<div class="flex items-baseline flex-col md:flex-row">
						<h2 class="text-2xl font-semibold mr-2">{name} Doe</h2>
						<span class="text-gray-700">Someplace, Somewhere</span>
					</div>
					<div class="flex pb-1">
						<span class="font-semibold text-blue-500"> XX References </span>						
					</div>
					<span>
						Working at John Doe's place was a great experience, consectetur adipiscing elit. Morbi in mauris
						sed nisl interdum pellentesque at ac arcu. Morbi pretium quis arcu eget luctus.
						Suspendisse aliquam, leo at malesuada feugiat, nunc lorem bibendum ante, a posuere quam
						urna a neque. Integer vel eros vitae lectus molestie placerat.	
					</span>
				</div>
			</div>
		</a>
	{/each}
</Card>
