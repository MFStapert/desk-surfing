<script lang="ts">
	import Card from '$lib/components/Card.svelte';
	import Profile from '$lib/components/Profile.svelte';
</script>

<div class="flex flex-col md:flex-row">
	<Profile fullName="Jane Doe" photo="Jane" location="The Netherlands" />
	<div class="grow">
		<Card title="Leave a reference:">
			<span class="block mb-2 text-gray-700">Rating:</span>
			<select>
				<option>Negative</option>
				<option>Neutral</option>
				<option>Positive</option>
			</select>

			<span class="block mb-2 text-gray-700">Reference:</span>
			<textarea rows="6" placeholder="Tell us about your time working with Jane Doe" />

			<button
				slot="controls"
				class=" bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded"
			>
				Reference
			</button>
		</Card>
	</div>
</div>
