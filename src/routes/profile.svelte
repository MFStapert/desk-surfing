<script lang="ts">
	import Card from '$lib/components/Card.svelte';
	import Profile from '$lib/components/Profile.svelte';

	import { Icon, Annotation, Briefcase, Chat, Clock } from 'svelte-hero-icons';
</script>

<div class="flex flex-col md:flex-row">
	<Profile fullName="Jane Doe" photo="Jane" location="The Netherlands" />
	<div>
		<Card>
			<div class="flex flex-col md:items-baseline md:flex-row md:justify-between">
				<h2 class="text-2xl font-semibold text-green-500 mb-4">Has a place to work</h2>
				<div class="flex flex-col md:block">
					<a
						href="/reference"
						class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded md:mr-2 mb-2"
					>
						Reference
					</a>
					<a
						href="/message"
						class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded"
					>
						Message
					</a>
				</div>
			</div></Card
		>

		<Card title="Overview:">
			<div class="grid grid-cols-1 md:grid-cols-2">
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
		</Card>

		<Card title="About:">
			Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi in mauris sed nisl interdum
			pellentesque at ac arcu. Morbi pretium quis arcu eget luctus. Suspendisse aliquam, leo at
			malesuada feugiat, nunc lorem bibendum ante, a posuere quam urna a neque. Integer vel eros
			vitae lectus molestie placerat. Mauris tortor magna, commodo ac quam in, euismod scelerisque
			tortor. Nulla ac lorem vel lectus iaculis posuere eget feugiat diam. Suspendisse venenatis
			elit nec nibh tempus gravida. Quisque non efficitur nulla. Aliquam a nisi eros. Nunc sit amet
			odio in mi ultrices dapibus eu a metus. Vivamus rhoncus nisi faucibus varius bibendum.
			Curabitur eleifend scelerisque mattis. Integer nec efficitur felis. Aliquam lorem ligula,
			ultricies in maximus at, tincidunt nec lorem. Phasellus tempor commodo pharetra. Phasellus
			vulputate tortor augue, id pretium augue ultricies nec.
		</Card>
	</div>
</div>
