<script lang="ts">
	import Navbar from '@/partials/Navbar.svelte';
	import Footer from '@/partials/Footer.svelte';
	import { onMount } from 'svelte';
	
	let { children } = $props();

	onMount(() => {
		new PerformanceObserver((entryList) => {
			for (const entry of entryList.getEntries()) {
				console.log('Layout shift:', entry);
			}
		}).observe({type: 'layout-shift', buffered: true});
	})
</script>

<div class="bg-white text-jhc-dark top-0 mt-20 bottom-0 left-0 right-0 overflow-x-hidden">
	<div class="w-full h-full flex flex-col max-w-full">
		<Navbar />
		<main class="flex flex-col left-0 right-0 h-auto">
			{@render children()}
		</main>
		<Footer />
	</div>
</div>