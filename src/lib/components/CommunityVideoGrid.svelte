<section class="py-24 bg-white border-t border-gray-200 font-sans">
    <div class="max-w-7xl mx-auto px-4 text-center mb-16">
        <span class="text-[10px] font-bold text-gray-500 uppercase tracking-widest border border-gray-200 px-3 py-1.5 rounded-full bg-gray-50">Industry Compliance Forums</span>
        <h2 class="mt-8 text-5xl md:text-6xl font-serif-display text-gray-900">Precision pays off. <br/> Literally.</h2>
        <p class="mt-6 text-gray-600 max-w-2xl mx-auto">Join the leading CDOs in chemical distribution who are overcoming data chaos with mathematically verified document transformation.</p>
        <div class="mt-8">
            <a href="#" class="inline-flex items-center justify-center px-6 py-3 border border-transparent text-sm font-bold rounded bg-gray-900 text-white hover:bg-gray-800 transition-colors">
                Join the Compliance Forum ->
            </a>
        </div>
    </div>

    <!-- Video Grid (Mockup) -->
    <div class="max-w-7xl mx-auto px-4">
        <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
            {#each Array(8) as _, i}
            <div class="aspect-video bg-gray-200 rounded-lg overflow-hidden relative group cursor-pointer">
                <div class="w-full h-full bg-[#022c22] flex items-center justify-center text-white/20 font-bold text-xl">
                    SOLVATE
                </div>
                <div class="absolute inset-0 flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity bg-black/20">
                    <div class="w-10 h-10 bg-white rounded-full flex items-center justify-center">
                        <svg class="w-4 h-4 ml-0.5" fill="currentColor" viewBox="0 0 24 24"><path d="M8 5v14l11-7z"/></svg>
                    </div>
                </div>
                <div class="absolute bottom-2 left-2 text-[10px] text-white font-medium bg-black/40 px-2 py-1 rounded">
                    Case Study #{i+1}
                </div>
            </div>
            {/each}
        </div>
        
        <!-- Quote -->
        <div class="mt-12 flex flex-col md:flex-row items-center gap-8 max-w-5xl mx-auto">
            <div class="w-24 h-24 md:w-32 md:h-32 rounded-full overflow-hidden flex-shrink-0 border-2 border-gray-100 bg-gray-200 flex items-center justify-center font-bold text-gray-400">
                SJ
            </div>
            <div class="flex-1 text-center md:text-left">
                <blockquote class="text-2xl md:text-3xl font-serif-display text-[#00ff66] leading-tight">
                    "Solvate's approach to document verification is a game-changer for the industry. It's the first time we've seen AI handle chemical data with this level of precision."
                </blockquote>
                <div class="mt-4 text-xs font-bold uppercase tracking-widest text-gray-400">
                    Sarah Jenkins <br/>
                    <span class="text-gray-300">Head of Supply Chain, Azelis</span>
                </div>
            </div>
        </div>
    </div>
</section>
