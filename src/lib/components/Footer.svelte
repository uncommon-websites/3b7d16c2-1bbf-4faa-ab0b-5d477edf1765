<script lang="ts">
    // Footer component
</script>

<footer class="bg-[#022c22] text-white pt-32 pb-12 overflow-hidden relative font-sans">
    <div class="max-w-7xl mx-auto px-4 relative z-10">
        <div class="text-center mb-24">
             <span class="text-[10px] font-bold uppercase tracking-widest border border-white/20 px-3 py-1.5 rounded-full mb-8 inline-block">Architecture Sessions</span>
             <h2 class="text-5xl md:text-7xl font-serif-display mb-6">Verified records,<br/> at enterprise scale.</h2>
             <p class="text-gray-400 mb-10 max-w-lg mx-auto text-sm">Work directly with our expert team to automate your document transformation gameplan and scale your operations with precision.</p>
             
             <div class="flex flex-col sm:flex-row justify-center gap-2 max-w-md mx-auto">
                 <input type="email" placeholder="Enter your work email" class="bg-white/5 border border-white/10 rounded-lg px-4 py-3 w-full text-white placeholder-gray-500 focus:outline-none focus:border-[#00ff66] transition-colors" />
                 <button class="bg-[#00ff66] hover:bg-[#00e05a] text-gray-900 px-6 py-3 rounded-lg font-bold whitespace-nowrap transition-colors flex items-center justify-center">
                     Book a Demo 
                     <svg class="w-4 h-4 ml-1" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14 5l7 7m0 0l-7 7m7-7H3"></path></svg>
                 </button>
             </div>
        </div>

        <div class="grid md:grid-cols-4 gap-12 border-t border-white/10 pt-16">
            <div>
                <h3 class="font-bold mb-6">Frequently Asked Questions</h3>
            </div>
            <div class="md:col-span-3 space-y-6">
                {#each ['How is Solvate different from generic OCR tools?', 'What chemical document types can Solvate process?', 'How does the three-layer validation work?', 'Can Solvate integrate with my existing SAP/Oracle ERP?', 'What is the accuracy rate for CAS and GHS data?'] as q}
                <div class="border-b border-white/10 pb-6 flex justify-between items-center cursor-pointer group">
                    <span class="text-lg font-light group-hover:text-[#00ff66] transition-colors">{q}</span>
                    <span class="text-2xl font-light">+</span>
                </div>
                {/each}
            </div>
        </div>

        <div class="grid grid-cols-2 md:grid-cols-5 gap-8 mt-24 text-sm text-gray-400">
            <div>
                <h4 class="text-white font-bold mb-4">Technology</h4>
                <ul class="space-y-2">
                    <li><a href="#" class="hover:text-white">AI Architecture</a></li>
                    <li><a href="#" class="hover:text-white">Three-Layer Validation</a></li>
                    <li><a href="#" class="hover:text-white">Integrations</a></li>
                    <li><a href="#" class="hover:text-white">Security</a></li>
                    <li><a href="#" class="hover:text-white">API Docs</a></li>
                </ul>
            </div>
            <div>
                <h4 class="text-white font-bold mb-4">Solutions</h4>
                <ul class="space-y-2">
                    <li><a href="#" class="hover:text-white">Chemical Distribution</a></li>
                    <li><a href="#" class="hover:text-white">Compliance Automation</a></li>
                    <li><a href="#" class="hover:text-white">Supply Chain Transparency</a></li>
                    <li><a href="#" class="hover:text-white">Data Transformation</a></li>
                </ul>
            </div>
            <div>
                <h4 class="text-white font-bold mb-4">Company</h4>
                <ul class="space-y-2">
                    <li><a href="#" class="hover:text-white">About Us</a></li>
                    <li><a href="#" class="hover:text-white">Careers</a></li>
                    <li><a href="#" class="hover:text-white">Contact</a></li>
                    <li><a href="#" class="hover:text-white">Partners</a></li>
                </ul>
            </div>
            <div>
                <h4 class="text-white font-bold mb-4">Resources</h4>
                <ul class="space-y-2">
                    <li><a href="#" class="hover:text-white">Compliance Forum</a></li>
                    <li><a href="#" class="hover:text-white">Case Studies</a></li>
                    <li><a href="#" class="hover:text-white">Industry Research</a></li>
                    <li><a href="#" class="hover:text-white">Whitepapers</a></li>
                </ul>
            </div>
            <div>
                <h4 class="text-white font-bold mb-4">Support</h4>
                <ul class="space-y-2">
                    <li><a href="#" class="hover:text-white">Help Center</a></li>
                    <li><a href="#" class="hover:text-white">Community</a></li>
                    <li><a href="#" class="hover:text-white">Status</a></li>
                </ul>
            </div>
        </div>
        
        <div class="mt-32 text-center relative">
             <h1 class="text-[12rem] md:text-[16rem] font-bold tracking-tighter leading-none text-white select-none">solvate</h1>
             <div class="absolute bottom-4 right-0 flex gap-4 text-[10px] text-gray-500 uppercase tracking-widest">
                 <a href="#">Privacy Policy</a>
                 <a href="#">Terms</a>
                 <a href="#">Contact</a>
             </div>
        </div>
    </div>
</footer>
