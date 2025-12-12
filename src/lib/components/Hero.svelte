<script lang="ts">
	import { ArrowRight, Menu } from 'lucide-svelte';
</script>

<section class="relative min-h-[600px] w-full overflow-hidden bg-[#2B95E0] text-white">
	<!-- Background Image / Gradient Simulation -->
	<div class="absolute inset-0 z-0">
        <!-- Base blue -->
		<div class="absolute inset-0 bg-gradient-to-br from-[#4facfe] to-[#00f2fe] opacity-80 mix-blend-multiply"></div>
        <div class="absolute inset-0 bg-[url('https://images.unsplash.com/photo-1506748686214-e9df14d4d9d0?q=80&w=2560&auto=format&fit=crop')] bg-cover bg-center mix-blend-overlay opacity-50"></div>
        <!-- Fallback gradient if image fails or for better tint -->
        <div class="absolute inset-0 bg-gradient-to-b from-blue-400/80 via-blue-500/80 to-blue-600/90"></div>
	</div>

	<!-- Content -->
	<div class="relative z-10 mx-auto max-w-7xl px-6 pt-8 pb-20 lg:px-8">
		<!-- Navigation -->
		<nav class="flex items-center justify-between">
			<!-- Logo -->
			<div class="flex items-center">
				<div class="flex h-10 w-10 items-center justify-center border-2 border-white text-xl font-bold font-display tracking-tighter">
					RC
				</div>
			</div>

			<!-- Desktop Menu -->
			<div class="hidden md:flex items-center gap-8 text-sm font-medium tracking-wide">
				<a href="#" class="hover:text-blue-100 transition-colors">Metrics</a>
				<a href="#" class="hover:text-blue-100 transition-colors">Services</a>
				<a href="#" class="hover:text-blue-100 transition-colors">Gateways</a>
				<a href="#" class="hover:text-blue-100 transition-colors">Transactions</a>
				<a href="#" class="hover:text-blue-100 transition-colors">About Us</a>
				<a href="#" class="hover:text-blue-100 transition-colors">Contact Us</a>
			</div>
            
            <!-- Mobile Menu Button -->
            <button class="md:hidden text-white">
                <Menu size={24} />
            </button>
		</nav>

		<!-- Hero Text -->
		<div class="mt-24 max-w-3xl">
			<h1 class="font-display text-5xl md:text-6xl lg:text-7xl leading-tight font-medium">
				Private Credit, Debt Advisory <br />
				& Strategic Capital Solutions
			</h1>
			<p class="mt-6 text-lg md:text-xl text-blue-50 font-light max-w-xl">
				Expertly structuring debt and funding solutions for all your deals.
			</p>

			<div class="mt-10">
				<button class="group flex items-center gap-2 rounded-full bg-white px-6 py-3 text-sm font-semibold text-blue-600 transition-all hover:bg-blue-50">
					Request More Info
					<ArrowRight class="h-4 w-4 transition-transform group-hover:translate-x-1" />
				</button>
			</div>
		</div>
	</div>

    <!-- Bottom Right Label -->
    <div class="absolute bottom-8 right-8 z-10 hidden md:flex items-center gap-3 text-white/90">
        <svg class="w-6 h-6" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
            <path d="M2 8h20" />
            <path d="M2 12h20" />
            <path d="M2 16h20" />
            <path d="M2 12c0 0 0-4 4-4s4 4 4 4 0-4 4-4 4 4 4 4 0-4 4-4" style="display:none"/> <!-- hiding complex path, using simple lines for 'Aligning' metaphor or just waves -->
            <!-- Actual waves -->
            <path d="M2 6c2-2 2-2 4 0s2 2 4 0 2-2 4 0 2 2 4 0 2-2 4 0" />
            <path d="M2 12c2-2 2-2 4 0s2 2 4 0 2-2 4 0 2 2 4 0 2-2 4 0" />
            <path d="M2 18c2-2 2-2 4 0s2 2 4 0 2-2 4 0 2 2 4 0 2-2 4 0" />
        </svg>
        <span class="text-sm font-medium tracking-wide">Aligning Capital</span>
    </div>
</section>
