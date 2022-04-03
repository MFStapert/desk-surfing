<script lang="ts">
	import Card from '$lib/components/Card.svelte';
	import Profile from '$lib/components/Profile.svelte';
</script>

<Profile fullName="Jane Doe" photo="Jane" location="The Netherlands" />

<Card>
	<div class="p-4 bg-slate-100">
		<span class="font-semibold mb-1"
			>You<span class="font-normal text-gray-800 mx-2">| 23:50</span></span
		>
		<p>I was wondering if I can come work at your place?</p>
		<p>Say next week tuesday from 09:00 - 17:00</p>
		<p>I have coffee!</p>
	</div>
	<div class="p-4">
		<span class="font-semibold mb-1"
			>Jane<span class="font-normal text-gray-800 mx-2">| 23:50</span></span
		>

		<p>Sure I'd be happy to host you!</p>
		<p>I got coffee, maybe bring some snacks :)?</p>
	</div>
</Card>

<Card title="Chat">
	<textarea rows="2" placeholder="Type your message here" />
	<button
		slot="controls"
		class=" bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded"
	>
		Send
	</button>
</Card>
