<script lang="ts">
	import { Shield, Users, TrendingUp, Layers, Zap, Briefcase } from 'lucide-svelte';

	const features = [
		{
			icon: Shield,
			title: 'Capital Secured',
			description: 'Over $7B in structured financing across debt, private credit, and growth capital.'
		},
		{
			icon: Users,
			title: 'Expanding Lender & Investor Network',
			description: '2,100+ direct lenders, investors, credit funds, and capital partners aligned with client needs.'
		},
		{
			icon: TrendingUp,
			title: 'Consistent Network Expansion',
			description: '15% annual growth, enhancing access to exclusive referral, lender & investor opportunities.'
		},
		{
			icon: Layers,
			title: 'Strategic Capital Structuring',
			description: 'Custom financing programs designed to fill capital gaps and optimize funding.'
		},
		{
			icon: Zap,
			title: 'Faster Funding Execution',
			description: 'Proprietary processes streamline transactions, reducing funding timelines by 30%.'
		},
		{
			icon: Briefcase,
			title: 'Proven Deal-Making Expertise',
			description: '85+ years of combined experience structuring complex financing solutions.'
		}
	];
</script>

<section class="bg-white py-24">
	<div class="mx-auto max-w-7xl px-6 lg:px-8">
		<div class="max-w-3xl">
			<h2 class="font-display text-4xl font-medium text-gray-900 sm:text-5xl">
				Structuring Capital, Filling Gaps, <br />
				and Driving Deals Forward
			</h2>
			<p class="mt-6 text-lg leading-8 text-gray-600">
				Raiseview Capital builds and executes financing solutions by structuring debt, optimizing capital stacks, and securing private credit. We connect businesses, dealmakers, and investors with the right funding sources. Whether for acquisitions, expansion, or liquidity, ensuring every deal is structured for success.
			</p>
		</div>

		<div class="mx-auto mt-16 grid max-w-2xl grid-cols-1 gap-x-8 gap-y-16 sm:mt-20 sm:grid-cols-2 lg:mx-0 lg:max-w-none lg:grid-cols-3">
			{#each features as feature}
				<div class="flex flex-col">
					<div class="mb-6 flex h-10 w-10 items-center justify-center rounded bg-blue-100 text-blue-600">
						<svelte:component this={feature.icon} class="h-6 w-6" />
					</div>
					<h3 class="font-display text-xl font-medium leading-7 text-gray-900">
						{feature.title}
					</h3>
					<p class="mt-3 text-sm leading-6 text-gray-600">
						{feature.description}
					</p>
				</div>
			{/each}
		</div>
	</div>
</section>
