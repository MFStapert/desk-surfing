<script lang="ts">
	import Card from '$lib/components/Card.svelte';
	import { Icon, Annotation, Briefcase, Chat, Clock } from 'svelte-hero-icons';
</script>

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

	<span for="formFile" class="block mb-2 text-gray-700">Upload pictures of your office</span>
	<input type="file" id="formFile" />

	<button
		slot="controls"
		class=" bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded"
	>
		Host
	</button>
</Card>
