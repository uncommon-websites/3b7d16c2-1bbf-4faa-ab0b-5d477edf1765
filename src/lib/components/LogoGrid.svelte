<script lang="ts">
    const logos = [
        { name: 'Brenntag', hasCaseStudy: false },
        { name: 'Univar', hasCaseStudy: true, caseStudyText: 'CASE STUDY' },
        { name: 'Helm AG', hasCaseStudy: false },
        { name: 'Tricon', hasCaseStudy: true, icon: true, caseStudyText: 'CASE STUDY' },
        { name: 'IMCD', hasCaseStudy: true, caseStudyText: 'CASE STUDY' },
        { name: 'Azelis', hasCaseStudy: false },
        { name: 'Biesterfeld', hasCaseStudy: false },
        { name: 'DKSH', hasCaseStudy: false, icon: true },
        { name: 'Stockmeier', hasCaseStudy: false },
        { name: 'Omya', hasCaseStudy: false },
        { name: 'Nordmann', hasCaseStudy: false },
        { name: 'logo_circle', hasCaseStudy: false, isImage: true }, // Placeholder for the black circle logo
        { name: 'Caldic', hasCaseStudy: false, icon: true },
        { name: 'Safic-Alcan', hasCaseStudy: false, icon: true },
        { name: 'Oqema', hasCaseStudy: false }
    ];
</script>

<section class="py-12 bg-white border-b border-gray-200 font-sans">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <p class="text-center text-[10px] uppercase tracking-widest text-[#00ff66] font-bold mb-8">
            TRUSTED BY THE WORLD'S LEADING CHEMICAL DISTRIBUTORS
        </p>

        <div class="grid grid-cols-2 md:grid-cols-5 gap-0 border-t border-l border-gray-200">
            {#each logos as logo}
                <div class="flex items-center justify-center p-6 border-r border-b border-gray-200 h-24 relative group">
                    <!-- Logo Placeholder -->
                    {#if logo.isImage}
                        <div class="w-8 h-8 rounded-full bg-black text-white flex items-center justify-center font-bold text-xs">
                            <svg class="w-4 h-4" fill="currentColor" viewBox="0 0 24 24"><path d="M12 2L2 7l10 5 10-5-10-5zm0 9l2.5-1.25L12 8.5l-2.5 1.25L12 11zm0 2.5l-5-2.5-5 2.5L12 22l10-8.5-5-2.5-5 2.5z"/></svg>
                        </div>
                    {:else}
                        <span class="text-xl md:text-2xl font-bold text-gray-400 group-hover:text-gray-900 transition-colors flex items-center gap-2">
                            {#if logo.icon}
                            <!-- Generic Icon for some -->
                            <div class="w-6 h-6 bg-gray-300 rounded-sm"></div>
                            {/if}
                            {logo.name}
                        </span>
                    {/if}

                    {#if logo.hasCaseStudy}
                        <a href="#" class="absolute top-2 right-2 text-[8px] font-bold text-emerald-600 bg-emerald-50 px-1.5 py-0.5 rounded border border-emerald-100 hover:bg-emerald-100 flex items-center transition-colors">
                            {logo.caseStudyText} 
                            <svg class="w-2 h-2 ml-0.5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"></path></svg>
                        </a>
                    {/if}
                </div>
            {/each}
        </div>
    </div>
</section>
