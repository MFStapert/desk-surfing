<script lang="ts">
	import Card from '$lib/components/Card.svelte';
	import { Icon, Annotation, Briefcase, Chat, Clock } from 'svelte-hero-icons';
</script>

<div class="flex">
	<Card title="Host an office:">
		<span class="block mb-2 text-gray-700">Days available:</span>
		<select class="mb-4">
			<option>Monday</option>
			<option>Tuesday</option>
			<option>Wednesday</option>
			<option>Thursday</option>
			<option>Friday</option>
			<option>Saturday</option>
			<option>Sunday</option>
		</select>

		<span class="block mb-2 text-gray-700">Description:</span>
		<textarea
			class=" mb-4"
			rows="6"
			placeholder="Tell something about yourself and your office space"
		/>

		<div class="mb-3 w-96">
			<label for="formFile" class="form-label inline-block mb-2 text-gray-700"
				>Upload pictures of your office</label
			>
			<input
				class="form-control
			  block
			  w-full
			  px-3
			  py-1.5
			  text-base
			  font-normal
			  text-gray-700
			  bg-white bg-clip-padding
			  border border-solid border-gray-300
			  rounded
			  transition
			  ease-in-out
			  m-0
			  focus:text-gray-700 focus:bg-white focus:border-blue-600 focus:outline-none"
				type="file"
				id="formFile"
			/>
		</div>

		<button
			slot="controls"
			class=" bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded"
		>
			Host
		</button>
	</Card>
</div>
