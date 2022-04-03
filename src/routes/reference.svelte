<script lang="ts">
	import Card from '$lib/components/Card.svelte';
	import InputWrapper from '$lib/components/InputWrapper.svelte';
	import Profile from '$lib/components/Profile.svelte';
</script>

<div class="flex flex-col md:flex-row">
	<Profile fullName="Jane Doe" photo="Jane" location="The Netherlands" />
	<div class="grow">
		<Card title="Leave a reference">
			<InputWrapper title="Rating">
				<select>
					<option>Positive</option>
					<option>Neutral</option>
					<option>Negative</option>
				</select>
			</InputWrapper>
			<InputWrapper title="Reference">
				<textarea rows="6" placeholder="Something aqbout your time working" />
			</InputWrapper>
			<button
				slot="controls"
				class=" bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded"
			>
				Reference
			</button>
		</Card>
	</div>
</div>
