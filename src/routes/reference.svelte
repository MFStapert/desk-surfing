<script lang="ts">
	import Card from '$lib/components/Card.svelte';
	import { Icon, Annotation, Briefcase, Chat, Clock } from 'svelte-hero-icons';
	import { text } from 'svelte/internal';
</script>

<div class="flex">
	<div class="flex flex-col min-w-fit min-h-screen m-2 p-4 rounded bg-white items-center space-x-4">
		<img
			src="Jane.jpg"
			alt=""
			class="flex-none w-32 h-32 rounded-full object-cover"
			loading="lazy"
		/>

		<h2 class="text-2xl font-semibold">Jane Doe</h2>
		<span class="text-blue-500 mt-0.5">Kaapstad, Zuid Afrika</span>
	</div>
	<div class="grow">
		<Card title="Leave a reference:">
			<span class="block mb-2 text-gray-700">Rating:</span>
			<select>
				<option>Negative</option>
				<option>Neutral</option>
				<option>Positive</option>
			</select>

			<span class="block mb-2 text-gray-700">Reference:</span>
			<textarea
				class="p-2 border border-gray-300 border-solid w-full rounded-md focus:text-gray-700 focus:bg-white focus:border-blue-600 focus:outline-none"
				rows="6"
				placeholder="Tell us about your time working with Jane Doe"
			/>

			<button
				slot="controls"
				class=" bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded"
			>
				Reference
			</button>
		</Card>
	</div>
</div>
