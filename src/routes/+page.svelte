<script lang="ts">
	import Hero from "$lib/components/Hero.svelte";
	import Features from "$lib/components/Features.svelte";
	import NetworkProfiles from "$lib/components/NetworkProfiles.svelte";
	import Services from "$lib/components/Services.svelte";
	import Gateways from "$lib/components/Gateways.svelte";
	import Transactions from "$lib/components/Transactions.svelte";
	import About from "$lib/components/About.svelte";
	import FastTrack from "$lib/components/FastTrack.svelte";
	import Footer from "$lib/components/Footer.svelte";
</script>

<div class="font-body text-gray-900 antialiased selection:bg-blue-200 selection:text-blue-900">
	<Hero />
	<Features />
	<NetworkProfiles />
	<Services />
	<Gateways />
	<Transactions />
	<About />
	<FastTrack />
	<Footer />
</div>

