<script lang="ts">
	import { Home, Circle, ArrowUp, Shuffle, Network, Layers, ArrowRight } from 'lucide-svelte';

	const rpnFeatures = [
		{
			icon: Home,
			title: 'Increase Sales & Deal Volume',
			description: 'We help your clients secure financing, removing a major barrier to closing more deals. More approved financing means more transactions completed and higher sales for you.'
		},
		{
			icon: Circle,
			title: 'End-to-End Funding Support',
			description: 'Our team sources lenders, structures financing, and ensures deals get funded, so you can focus on selling while we handle the financial execution.'
		},
		{
			icon: ArrowUp,
			title: 'Stronger Client Relationships',
			description: 'By offering a seamless financing solution, you position yourself as a trusted partner who not only provides great products or services but also helps clients get the capital they need to move forward.'
		}
	];

	const irnFeatures = [
		{
			icon: Shuffle,
			title: 'Dynamic Investor Pool',
			description: 'A growing network of institutional investors, family offices, and private financiers gains direct access to off-market opportunities tailored to their investment focus.'
		},
		{
			icon: Network,
			title: 'Strategic Connectivity',
			description: 'Our clients\' capital-raising initiatives are aligned with investor mandates, ensuring relevant and actionable deal flow. Investors engage with vetted opportunities, maximizing time efficiency and investment potential.'
		},
		{
			icon: Layers,
			title: 'Dual Value Creation',
			description: 'The IRN delivers value to clients by ensuring their funding needs are matched with the right investors, while investors gain curated access to high-quality deals sourced from Raiseview\'s global pipeline.'
		}
	];
</script>

<section class="bg-white py-24">
	<div class="mx-auto max-w-7xl px-6 lg:px-8">
		<h2 class="font-display text-4xl font-medium text-gray-900 mb-16">Network Gateways</h2>

		<!-- RPN Section -->
		<div class="mb-24">
			<h3 class="font-display text-2xl font-medium text-gray-900 mb-4">Referral Partner Network (RPN)</h3>
			<p class="max-w-4xl text-gray-600 mb-12">
				The Referral Partner Network connects distributors, manufacturers, vendors, M&A firms, investment banks, private lenders, and marketing agencies with a proven system to increase sales, accelerate deal closings, and secure more funded transactions. Our partners refer clients needing financing, and we ensure they get the capital required to close.
			</p>

			<div class="grid grid-cols-1 gap-8 md:grid-cols-3">
				{#each rpnFeatures as feature}
					<div class="rounded-2xl border border-gray-100 bg-gray-50/50 p-8">
						<div class="mb-6 flex h-10 w-10 items-center justify-center rounded-full bg-blue-100 text-blue-600">
							<svelte:component this={feature.icon} class="h-5 w-5" />
						</div>
						<h4 class="font-display text-lg font-medium text-gray-900 mb-3">{feature.title}</h4>
						<p class="text-sm leading-relaxed text-gray-600">{feature.description}</p>
					</div>
				{/each}
			</div>

            <div class="mt-10 text-center">
                 <p class="text-sm text-gray-500 mb-4">If you work with businesses that need funding to complete purchases or transactions, partner with us and turn more opportunities into closed deals.</p>
                 <button class="inline-flex items-center gap-2 rounded-full bg-blue-50 px-6 py-2.5 text-sm font-semibold text-blue-600 hover:bg-blue-100 transition-colors">
                    <span class="flex h-5 w-5 items-center justify-center rounded-full bg-blue-200 text-blue-700">
                        <ArrowRight class="h-3 w-3" />
                    </span>
                    Join the Network
                 </button>
            </div>
		</div>

		<!-- IRN Section -->
		<div>
			<h3 class="font-display text-2xl font-medium text-gray-900 mb-4">Investor Rolodex Network (IRN)</h3>
			<p class="max-w-4xl text-gray-600 mb-12">
				The Investor Rolodex Network bridges qualified investors with exclusive off-market opportunities sourced through Raiseview's extensive client base. This program continuously evolves with strategic relationships, ensuring access to deals aligned with precise mandates. By actively enrolling investors and leveraging our global network, we create a seamless flow of opportunities that benefits both investors and clients.
			</p>

			<div class="grid grid-cols-1 gap-8 md:grid-cols-3">
				{#each irnFeatures as feature}
					<div class="rounded-2xl border border-gray-100 bg-gray-50/50 p-8">
						<div class="mb-6 flex h-10 w-10 items-center justify-center rounded bg-blue-100 text-blue-600">
							<svelte:component this={feature.icon} class="h-5 w-5" />
						</div>
						<h4 class="font-display text-lg font-medium text-gray-900 mb-3">{feature.title}</h4>
						<p class="text-sm leading-relaxed text-gray-600">{feature.description}</p>
					</div>
				{/each}
			</div>

            <div class="mt-10 text-center">
                 <button class="inline-flex items-center gap-2 rounded-full bg-blue-50 px-6 py-2.5 text-sm font-semibold text-blue-600 hover:bg-blue-100 transition-colors">
                    <span class="flex h-5 w-5 items-center justify-center rounded-full bg-blue-200 text-blue-700">
                        <ArrowRight class="h-3 w-3" />
                    </span>
                    Join Us for Exclusive Opportunities
                 </button>
            </div>
		</div>
	</div>
</section>
