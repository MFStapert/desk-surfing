<script lang="ts">
	import Card from '$lib/components/Card.svelte';
	import InputWrapper from '$lib/components/InputWrapper.svelte';
</script>

<Card title="Profile">
	<InputWrapper title="Firstname">
		<input />
	</InputWrapper>

	<InputWrapper title="Lastname">
		<input />
	</InputWrapper>

	<InputWrapper title="Country of birth">
		<input />
	</InputWrapper>

	<InputWrapper title="Languages">
		<input />
	</InputWrapper>

	<InputWrapper title="Date of birth">
		<input />
	</InputWrapper>

	<InputWrapper title="Profile picture">
		<input type="file" id="formFile" />
	</InputWrapper>

	<InputWrapper title="Bio">
		<textarea rows="6" placeholder="Tell something about yourself" />
	</InputWrapper>

	<button
		slot="controls"
		class=" bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded"
	>
		Save
	</button>
</Card>
