<script lang="ts">
	const profiles = [
		"Endowments and Foundations",
		"Sovereign Wealth and Pension Funds",
		"Insurance Firms and Fund of Funds",
		"High-Net-Worth (HNW) Individuals",
		"Single Family Offices",
        "Sovereign & Pension-Backed Credit Investors",
        "Infrastructure & Project Finance Lenders",
        "Ultra-High-Net-Worth Individuals (UHNWIs)",
        "Private Equity Firms"
	];
</script>

<section class="bg-white pb-16 pt-4 border-t border-gray-100">
	<div class="mx-auto max-w-7xl px-6 lg:px-8">
		<h3 class="font-display text-2xl font-medium text-gray-900 mb-8">Our Network Profiles:</h3>
		
        <!-- Scrolling Container -->
        <div class="relative w-full overflow-hidden">
            <!-- Fade masks -->
            <div class="pointer-events-none absolute left-0 top-0 bottom-0 w-20 bg-gradient-to-r from-white to-transparent z-10"></div>
            <div class="pointer-events-none absolute right-0 top-0 bottom-0 w-20 bg-gradient-to-l from-white to-transparent z-10"></div>

            <div class="flex overflow-x-auto pb-4 scrollbar-hide gap-4 no-scrollbar items-center">
                {#each profiles as profile}
                    <div class="flex-none rounded-full border border-gray-200 bg-gray-50 px-6 py-2 text-sm text-gray-600 whitespace-nowrap hover:border-gray-300 hover:bg-gray-100 transition-colors cursor-default">
                        {profile}
                    </div>
                {/each}
                 <!-- Duplicate for length if needed, or just let it scroll -->
                 {#each profiles as profile}
                    <div class="flex-none rounded-full border border-gray-200 bg-gray-50 px-6 py-2 text-sm text-gray-600 whitespace-nowrap hover:border-gray-300 hover:bg-gray-100 transition-colors cursor-default">
                        {profile}
                    </div>
                {/each}
            </div>
        </div>
	</div>
</section>

<style>
    /* Hide scrollbar for Chrome, Safari and Opera */
    .no-scrollbar::-webkit-scrollbar {
        display: none;
    }
    /* Hide scrollbar for IE, Edge and Firefox */
    .no-scrollbar {
        -ms-overflow-style: none;  /* IE and Edge */
        scrollbar-width: none;  /* Firefox */
    }
</style>
