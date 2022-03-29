<script lang="ts">
	import { Icon, Annotation, Briefcase, Chat, Clock } from 'svelte-hero-icons';
</script>

<div class="flex bg-slate-50">
	<div class="flex flex-col min-h-screen m-2 p-4 rounded bg-white items-center space-x-4">
		<img
			src="profile.jpg"
			alt=""
			class="flex-none w-32 h-32 rounded-full object-cover"
			loading="lazy"
		/>

		<h2 class="text-2xl font-semibold">Jane Doe</h2>
		<span class="text-blue-500 mt-0.5">Kaapstad, Zuid Afrika</span>
	</div>

	<div class="grow h-fit m-2 rounded bg-white">
		<div class="p-4 border-b-2 border-slate-50">
			<h2 class="text-2xl font-semibold">Overview</h2>
		</div>
		<div class="p-4 grid grid-cols-2">
			<div class="flex mb-6">
				<Icon solid src={Annotation} class="h-6 w-6 mr-2 blue-300 text-blue-500 " />
				<span class="font-semibold text-blue-500"> 14 References </span>
			</div>
			<div class="flex mb-6">
				<Icon solid src={Briefcase} class="h-6 w-6 mr-2 blue-300 text-gray-600" />
				<span class="font-semibold text-gray-600"> Software engineer </span>
			</div>
			<div class="flex mb-6">
				<Icon solid src={Chat} class="h-6 w-6 mr-2 blue-300 text-gray-600 " />
				<span class="font-semibold text-gray-600"> Dutch </span>
			</div>
			<div class="flex mb-6">
				<Icon solid src={Clock} class="h-6 w-6 mr-2 blue-300 text-gray-600 " />
				<span class="font-semibold text-gray-600"> 20 years old </span>
			</div>
		</div>
	</div>
</div>
