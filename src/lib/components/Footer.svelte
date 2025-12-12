<script lang="ts">
    import { Linkedin, Facebook, Instagram, Twitter } from 'lucide-svelte';
</script>

<footer class="relative overflow-hidden bg-[#0A2540] text-white pt-20 pb-0">
    <!-- Darker overlay/gradient -->
    <div class="absolute inset-0 bg-gradient-to-br from-[#0A2540] to-[#051220]"></div>

    <div class="relative z-10 mx-auto max-w-7xl px-6 lg:px-8">
        <div class="grid grid-cols-1 gap-12 lg:grid-cols-4 mb-24">
            <!-- Logo Column -->
            <div>
                <div class="mb-8 flex h-12 w-12 items-center justify-center border-2 border-white text-2xl font-bold font-display tracking-tighter">
                    RC
                </div>
            </div>

            <!-- Menu -->
            <div>
                <h3 class="text-sm font-semibold text-blue-200 mb-6">Menu</h3>
                <ul class="space-y-4 text-sm">
                    <li><a href="#" class="hover:text-blue-200 transition-colors">Metrics</a></li>
                    <li><a href="#" class="hover:text-blue-200 transition-colors">Services</a></li>
                    <li><a href="#" class="hover:text-blue-200 transition-colors">Gateways</a></li>
                    <li><a href="#" class="hover:text-blue-200 transition-colors">Transactions</a></li>
                    <li><a href="#" class="hover:text-blue-200 transition-colors">About Us</a></li>
                    <li><a href="#" class="hover:text-blue-200 transition-colors">Contact Us</a></li>
                </ul>
            </div>

            <!-- Services -->
            <div>
                <h3 class="text-sm font-semibold text-blue-200 mb-6">Services</h3>
                <ul class="space-y-4 text-sm">
                    <li><a href="#" class="hover:text-blue-200 transition-colors">Capital Raising & Relations</a></li>
                    <li><a href="#" class="hover:text-blue-200 transition-colors">Debt Advisory</a></li>
                    <li><a href="#" class="hover:text-blue-200 transition-colors">Deal Flow & Origination</a></li>
                    <li><a href="#" class="hover:text-blue-200 transition-colors">Growth Acceleration Program</a></li>
                </ul>
                
                <h3 class="text-sm font-semibold text-blue-200 mt-8 mb-6">Network Gateways</h3>
                <ul class="space-y-4 text-sm">
                    <li><a href="#" class="hover:text-blue-200 transition-colors">Referral Partner Network (RPN)</a></li>
                    <li><a href="#" class="hover:text-blue-200 transition-colors">Investor Rolodex Network (IRN)</a></li>
                </ul>
            </div>

            <!-- Office Locations -->
            <div>
                <h3 class="text-sm font-semibold text-blue-200 mb-6">Office Locations</h3>
                <div class="space-y-4 text-sm mb-8">
                    <p>777 Hornby St Vancouver, BC V6Z 1S4, Canada</p>
                    <p>30 N Gould St Ste R Sheridan, Wyoming, USA</p>
                </div>

                <h3 class="text-sm font-semibold text-blue-200 mb-6">Follow Us</h3>
                <div class="flex gap-4 text-sm mb-8">
                    <a href="#" class="hover:text-blue-200 transition-colors">LinkedIn</a>
                    <span class="text-blue-400">X</span>
                    <a href="#" class="hover:text-blue-200 transition-colors">Facebook</a>
                    <a href="#" class="hover:text-blue-200 transition-colors">Instagram</a>
                </div>

                <p class="text-sm font-semibold mb-4">info@raiseviewcapital.com</p>
                
                <div class="flex gap-4 text-xs text-blue-200">
                    <a href="#" class="hover:text-white transition-colors">Privacy Policy</a>
                    <a href="#" class="hover:text-white transition-colors">Terms of Service</a>
                </div>
            </div>
        </div>

        <div class="border-t border-blue-400/30 pt-8 pb-32 text-xs text-blue-200 space-y-4 max-w-3xl">
            <p>Copyright © 2024 Raiseview Capital | All Rights Reserved.</p>
            <p class="leading-relaxed opacity-70">
                Raiseview Capital (the "Raiseview Capital LLC Website") is operated by Raiseview Capital LLC, a privately held limited liability company. While not a registered broker-dealer, Raiseview Capital provides advisory services for capital raising, investor relations, M&A, and debt advisory, without engaging in securities transactions.
            </p>
        </div>
    </div>

    <!-- Big Text at Bottom -->
    <div class="absolute bottom-[-5vw] left-0 right-0 w-full overflow-hidden leading-none select-none pointer-events-none">
         <h1 class="text-[22vw] font-display font-medium text-white/10 text-center whitespace-nowrap tracking-tighter">
            Raiseview
         </h1>
    </div>
</footer>
