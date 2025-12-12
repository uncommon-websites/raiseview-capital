<script lang="ts">
	import { ArrowRight } from 'lucide-svelte';

	const options = [
		{
			title: 'Inquire About Our Services',
			description: 'Ready to elevate your capital-raising strategy?\n\nMeet with us for tailored solutions that maximize your funding potential.',
			cta: 'Connect',
            iconColor: 'bg-blue-500'
		},
		{
			title: 'Join Our Investor Network',
			description: 'Looking to access high-value investment opportunities?\n\nSubmit your mandates to join our growing network of strategic investors.',
			cta: 'Explore',
            iconColor: 'bg-blue-400'
		},
		{
			title: 'Become A Referral Partner',
			description: 'Join our Referral Partner Network (RPN) to help businesses secure financing, close more deals, and drive higher sales.\n\nFill out the form to become a trusted partner and collaborate on funding opportunities that turn referrals into closed transactions.',
			cta: 'Partner',
            iconColor: 'bg-blue-300'
		}
	];
</script>

<section class="bg-gray-50 py-24">
	<div class="mx-auto max-w-7xl px-6 lg:px-8">
		<h2 class="font-display text-4xl font-medium text-gray-900 mb-12">Fast Track Connections</h2>

		<div class="grid grid-cols-1 gap-8 md:grid-cols-3">
			{#each options as option}
				<div class="flex flex-col justify-between rounded-xl bg-white p-8 shadow-sm ring-1 ring-gray-900/5">
					<div>
						<h3 class="font-display text-2xl font-medium text-gray-900 mb-6">{option.title}</h3>
						<p class="whitespace-pre-line text-sm leading-relaxed text-gray-600 mb-8">
							{option.description}
						</p>
					</div>
					<button class="group flex items-center gap-2 text-sm font-semibold text-gray-900">
                        <div class="flex h-6 w-6 items-center justify-center rounded-full {option.iconColor} text-white transition-transform group-hover:scale-110">
                            <ArrowRight class="h-3 w-3" />
                        </div>
						{option.cta}
					</button>
				</div>
			{/each}
		</div>
	</div>
</section>
