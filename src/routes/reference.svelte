<script lang="ts">
	import { Icon, Annotation, Briefcase, Chat, Clock } from 'svelte-hero-icons';
	import { text } from 'svelte/internal';
</script>

<div class="flex">
	<div class="flex flex-col min-w-fit min-h-screen m-2 p-4 rounded bg-white items-center space-x-4">
		<img
			src="profile.jpg"
			alt=""
			class="flex-none w-32 h-32 rounded-full object-cover"
			loading="lazy"
		/>

		<h2 class="text-2xl font-semibold">Jane Doe</h2>
		<span class="text-blue-500 mt-0.5">Kaapstad, Zuid Afrika</span>
	</div>

	<div class="h-min w-full m-2 rounded bg-white">
		<div class="p-4 border-b-2 border-slate-50">
			<h2 class="text-2xl font-semibold">Leave a reference:</h2>
		</div>
		<div class="p-4 w-full">
			<span class="block mb-2 text-gray-700">Rating:</span>
			<select
				class="
			w-full
			px-3
			py-1.5
			text-base
			font-normal
			text-gray-700
			bg-white
			border border-solid border-gray-300
			rounded-md
			mb-2
			focus:text-gray-700 focus:bg-white focus:border-blue-600 focus:outline-none
			"
			>
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
		</div>
		<div class="flex flex-row-reverse p-4 border-t-2 border-slate-50">
			<button class=" bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
				Reference
			</button>
		</div>
	</div>
</div>
