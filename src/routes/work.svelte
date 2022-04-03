<script lang="ts">
	import Card from '$lib/components/Card.svelte';

	import { Icon, Search, Annotation, Briefcase, Chat, Clock } from 'svelte-hero-icons';
</script>

<Card title="Find a place to work:">
	<div class="flex align-baseline self-center p-2 mb-4 border rounded-md border-gray-400">
		<Icon solid src={Search} class="h-6  w-6 mr-2  text-gray-400" />
		<input class="border-none p-0 outline-none" placeholder="search by location" />
	</div>

	<div class="flex flex-col md:flex-row">
		<div class=" grow mr-0 md:mr-4">
			<span class="block mb-2 text-gray-700">Date from:</span>
			<input type="date" />
		</div>
		<div class="grow">
			<span class="block mb-2 text-gray-700">Date to:</span>
			<input type="date" />
		</div>
	</div>
</Card>

<Card title="Results:">
	{#each ['Janet', 'Jane', 'Jacky', 'Joe'] as name}
		<a href="profile">
			<div class="flex flex-row p-4 border-b border-slate-200">
				<img
					src="{name}.jpg"
					alt=""
					class="flex-none w-32 h-32 rounded-full object-cover mr-4"
					loading="lazy"
				/>
				<div class="flex flex-col w-full">
					<div class="flex items-baseline pb-1 border-b border-slate-200">
						<h2 class="text-2xl font-semibold mr-2">{name} Doe</h2>
						<span class="text-gray-600 mt-0.5">Kaapstad, Zuid Afrika</span>
					</div>
					<div class="flex pb-1 border-b border-slate-200">
						<span class="font-semibold text-blue-500"> 14 References </span>
						<span class="mx-2 font-semibold text-gray-600"> | </span>
						<span class="font-semibold text-gray-600"> Software engineer </span>
						<span class="mx-2 font-semibold text-gray-600"> | </span>
						<span class="font-semibold text-gray-600"> Dutch </span>
					</div>
					<span>
						I'm hosting people from monday to tuesday, consectetur adipiscing elit. Morbi in mauris
						sed nisl interdum pellentesque at ac arcu. Morbi pretium quis arcu eget luctus.
						Suspendisse aliquam, leo at malesuada feugiat, nunc lorem bibendum ante, a posuere quam
						urna a neque. Integer vel eros vitae lectus molestie placerat.
					</span>
				</div>
			</div>
		</a>
	{/each}
</Card>
