<script lang="ts">
	import Card from '$lib/components/Card.svelte';
	import InputWrapper from '$lib/components/InputWrapper.svelte';
	import { Icon, Annotation, Briefcase, Chat, Clock } from 'svelte-hero-icons';
</script>

<Card title="Host an place to work">
	<InputWrapper title="Days available">
		<select class="mb-4">
			<option>Monday</option>
			<option>Tuesday</option>
			<option>Wednesday</option>
			<option>Thursday</option>
			<option>Friday</option>
			<option>Saturday</option>
			<option>Sunday</option>
		</select>
	</InputWrapper>

	<InputWrapper title="Description">
		<textarea rows="6" placeholder="Tell something about  your office space" />
	</InputWrapper>

	<InputWrapper title="Upload pictures of your office">
		<input type="file" id="formFile" />
	</InputWrapper>

	<button
		slot="controls"
		class=" bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded"
	>
		Host
	</button>
</Card>
