<script lang="ts">
	import Card from '$lib/components/Card.svelte';
	import Profile from '$lib/components/Profile.svelte';
</script>

<Profile fullName="Jane Doe" photo="Jane" location="The Netherlands" />

<Card>
	<div class="flex flex-row-reverse p-4 font-semibold bg-green-100 border-b  border-slate-200 ">
		I was wondering if I can work at your place?
	</div>
	<div class="flex flex-row-reverse p-4 font-semibold bg-green-100 border-b  border-slate-200 ">
		Say next week tuesday from 09:00 - 17:00
	</div>
	<div class="flex flex-row-reverse p-4 font-semibold bg-green-100 border-b  border-slate-200 ">
		I have coffee!
	</div>

	<div class="p-4 border-b font-semibold border-slate-200">Sure I'd be happy to host you!</div>
	<div class="p-4 border-b font-semibold border-slate-200">
		I got coffee, maybe bring some snacks :)?
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
