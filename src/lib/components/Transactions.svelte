<script lang="ts">
	import { ChevronLeft, ChevronRight } from 'lucide-svelte';

	const transactions = [
		{
			category: 'Structured Debt',
			client: 'Biotech Firm',
			description: 'Secured $50M in structured debt. Accelerated clinical trials and R&D expansion.'
		},
		{
			category: 'Syndicated Loan',
			client: 'Private Equity Firm',
			description: 'Structured $200M in syndicated debt. Supported M&A activity in infrastructure.'
		},
		{
			category: 'Debt Financing',
			client: 'Clean Energy Initiative',
			description: 'Arranged $60M in debt financing. Developed renewable infrastructure and storage.'
		},
		{
			category: 'Project Financing',
			client: 'Renewable Energy Project',
			description: 'Arranged $35M in project financing. Funded solar farm construction and distribution.'
		},
		{
			category: 'Asset-Based Lending',
			client: 'Oil & Gas Exploration Firm',
			description: 'Closed $14M in asset-based lending. Expanded exploration and optimized production.'
		},
		{
			category: 'Expansion Capital',
			client: 'Healthcare Facilities Network',
			description: 'Secured $25M in expansion capital. Built new clinics and scaled telehealth.'
		}
	];
</script>

<section class="relative overflow-hidden bg-[#2B95E0] py-24 text-white">
    <!-- Background Gradient -->
    <div class="absolute inset-0 z-0 bg-gradient-to-br from-[#2B95E0] to-[#1a6db0]"></div>
    
	<div class="relative z-10 mx-auto max-w-7xl px-6 lg:px-8">
		<div class="mb-12 flex flex-col justify-between gap-8 md:flex-row md:items-end">
			<div class="max-w-2xl">
				<h2 class="font-display text-4xl font-medium mb-4">Recent Transactions</h2>
				<p class="text-blue-100 mb-4 font-medium">
					We uphold strict confidentiality to safeguard competitive strategies, ensuring client privacy by never disclosing company names or sensitive transaction details.
				</p>
                <p class="text-xs text-blue-200">
                    Case studies are available for board-level reviews or investment committee approvals.
                </p>
			</div>
			<div class="flex gap-2">
				<button class="rounded-full bg-white/10 p-2 hover:bg-white/20 transition-colors">
					<ChevronLeft class="h-6 w-6" />
				</button>
				<button class="rounded-full bg-white/10 p-2 hover:bg-white/20 transition-colors">
					<ChevronRight class="h-6 w-6" />
				</button>
			</div>
		</div>

		<div class="grid grid-cols-1 gap-6 md:grid-cols-2 lg:grid-cols-3">
			{#each transactions as transaction}
				<div class="flex flex-col justify-between rounded-lg bg-white p-8 text-gray-900 shadow-lg">
					<div>
						<div class="mb-4 flex items-center gap-2">
							<div class="h-2 w-2 rounded-full bg-blue-500"></div>
							<span class="text-xs font-semibold uppercase tracking-wider text-gray-500">{transaction.category}</span>
						</div>
						<h3 class="font-display text-xl font-medium mb-4">{transaction.client}</h3>
						<p class="text-sm leading-relaxed text-gray-600">{transaction.description}</p>
					</div>
				</div>
			{/each}
		</div>
	</div>
</section>
