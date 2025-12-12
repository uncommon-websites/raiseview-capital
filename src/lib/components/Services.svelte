<script lang="ts">
	import { ChevronLeft, ChevronRight } from 'lucide-svelte';

	const services = [
		{
			title: 'Debt & Credit Solutions',
			items: [
				'Term Loans',
				'Revolving Credit Facilities',
				'Working Capital Loans',
				'Bridge Loans',
				'Asset-Based Lending (ABL)'
			]
		},
		{
			title: 'Real Estate & Construction Loans',
			items: [
				'Commercial Real Estate (CRE) Loans',
				'Construction Loans',
				'Mezzanine Debt',
				'Owner-Occupied Real Estate Financing',
				'Mixed-Use & Multi-Family Property Loans'
			]
		},
		{
			title: 'Receivables & Inventory Financing',
			items: [
				'Invoice Factoring',
				'Accounts Receivable (A/R) Financing',
				'Purchase Order (PO) Financing',
				'Inventory Financing',
				'Supply Chain Financing'
			]
		},
		{
			title: 'Equipment & Vendor Financing',
			items: [
				'Equipment Leasing',
				'Vendor Financing Programs',
				'Sale-Leaseback Financing',
				'Machinery & Heavy Equipment Loans',
				'Transportation & Fleet Financing'
			]
		},
		{
			title: 'Acquisition & Expansion Financing',
			items: [
				'Acquisition Financing',
				'Leveraged Buyout (LBO) Loans',
				'Management Buyout (MBO) Financing',
				'Business Expansion Loans',
				'Growth Capital Loans'
			]
		},
		{
			title: 'Private Credit & Structured Finance',
			items: [
				'Private Credit Facilities',
				'Convertible Debt',
				'Syndicated Loans',
				'Structured Debt Placements',
				'Club Deals'
			]
		}
	];
</script>

<section class="bg-gray-50 py-24">
	<div class="mx-auto max-w-7xl px-6 lg:px-8">
		<div class="flex items-center justify-between mb-12">
			<h2 class="font-display text-4xl font-medium text-gray-900">Our Services</h2>
			<div class="flex gap-2">
				<button class="rounded-full border border-gray-200 bg-white p-2 text-gray-400 hover:text-gray-600 hover:border-gray-300 transition-colors">
					<ChevronLeft class="h-5 w-5" />
				</button>
				<button class="rounded-full border border-gray-200 bg-white p-2 text-gray-400 hover:text-gray-600 hover:border-gray-300 transition-colors">
					<ChevronRight class="h-5 w-5" />
				</button>
			</div>
		</div>

		<div class="grid grid-cols-1 gap-6 md:grid-cols-2 lg:grid-cols-3">
			{#each services as service}
				<div class="rounded-xl bg-white p-8 shadow-sm ring-1 ring-gray-900/5 transition-shadow hover:shadow-md">
					<h3 class="font-display text-xl font-medium text-gray-900 mb-6">{service.title}</h3>
					<ul class="space-y-3">
						{#each service.items as item}
							<li class="flex items-start gap-3 text-sm text-gray-600">
								<div class="mt-1.5 h-1.5 w-1.5 flex-none rounded-sm bg-blue-500"></div>
								<span>{item}</span>
							</li>
						{/each}
					</ul>
				</div>
			{/each}
		</div>
	</div>
</section>
