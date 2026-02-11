<script lang="ts">
    // No script logic needed for this static recreation yet
</script>

<section class="py-20 bg-white font-sans">
    <div class="max-w-7xl mx-auto px-4 text-center">
        <span class="text-[10px] font-bold text-gray-500 uppercase tracking-widest border border-gray-200 px-3 py-1.5 rounded-full bg-gray-50">The Solvate Architecture</span>
        <h2 class="mt-8 text-5xl md:text-7xl font-serif-display text-gray-900 leading-tight">From document chaos <br/> to verified <br/> records</h2>
    </div>
    
    <!-- Tabbed interface image area -->
    <div class="max-w-7xl mx-auto mt-16 px-4">
        <div class="border border-gray-200 rounded-xl overflow-hidden shadow-sm bg-white grid md:grid-cols-12 min-h-[600px]">
             <div class="md:col-span-4 p-8 md:p-12 border-r border-gray-200 flex flex-col justify-center">
                 <h3 class="text-3xl font-serif-display mb-4">Three-Layer AI Validation</h3>
                 <p class="text-gray-600 text-base leading-relaxed mb-8">Solvate doesn't just extract data; it verifies it. Our architecture uses three independent AI layers to cross-reference chemical properties, regulatory compliance, and manufacturer specs. This ensures 99.9% accuracy for your ERP and compliance systems.</p>
                 <div>
                    <button class="text-sm font-bold border-b border-gray-300 pb-0.5 hover:border-gray-900 transition-colors">Learn More -></button>
                 </div>
             </div>
             <div class="md:col-span-8 bg-gray-50 p-8 md:p-12 flex items-center justify-center relative overflow-hidden">
                 <!-- Simplified UI Mockup -->
                 <div class="bg-white shadow-xl rounded-lg w-full h-full border border-gray-200 p-6 relative flex flex-col">
                    <div class="flex gap-2 mb-6 border-b border-gray-100 pb-4">
                        <div class="w-3 h-3 rounded-full bg-red-400"></div>
                        <div class="w-3 h-3 rounded-full bg-yellow-400"></div>
                        <div class="w-3 h-3 rounded-full bg-green-400"></div>
                        <div class="ml-auto flex gap-2">
                            <div class="h-4 w-32 bg-gray-100 rounded-full"></div>
                        </div>
                    </div>
                    
                    <div class="space-y-6">
                        <!-- Header Stats -->
                        <div class="grid grid-cols-4 gap-4">
                             <div class="p-3 bg-gray-50 rounded border border-gray-100">
                                 <div class="text-[10px] text-gray-500 uppercase font-bold">Docs Processed</div>
                                 <div class="text-xl font-bold text-gray-900">8,420</div>
                                 <div class="text-[10px] text-green-600 font-bold">+24%</div>
                             </div>
                             <div class="p-3 bg-gray-50 rounded border border-gray-100">
                                 <div class="text-[10px] text-gray-500 uppercase font-bold">Accuracy</div>
                                 <div class="text-xl font-bold text-gray-900">99.98%</div>
                                 <div class="text-[10px] text-green-600 font-bold">Verified</div>
                             </div>
                             <div class="p-3 bg-gray-50 rounded border border-gray-100">
                                 <div class="text-[10px] text-gray-500 uppercase font-bold">Time Saved</div>
                                 <div class="text-xl font-bold text-gray-900">1,240h</div>
                                 <div class="text-[10px] text-green-600 font-bold">Monthly</div>
                             </div>
                             <div class="p-3 bg-gray-50 rounded border border-gray-100">
                                 <div class="text-[10px] text-gray-500 uppercase font-bold">Risk Score</div>
                                 <div class="text-xl font-bold text-gray-900">0.02</div>
                                 <div class="text-[10px] text-gray-400 font-bold">Low</div>
                             </div>
                        </div>

                        <!-- Data Table -->
                        <div class="border border-gray-100 rounded-lg overflow-hidden">
                            <div class="bg-gray-50 px-4 py-2 border-b border-gray-100 flex text-[10px] font-bold text-gray-500 uppercase tracking-wider">
                                <div class="w-1/3">Chemical Compound</div>
                                <div class="w-1/6 text-right">CAS No.</div>
                                <div class="w-1/6 text-right">Purity</div>
                                <div class="w-1/6 text-right">Source</div>
                                <div class="w-1/6 text-right">Status</div>
                            </div>
                            <div class="divide-y divide-gray-50 text-xs">
                                 {#each [
                                     {kw: 'Ethylene Glycol', vol: '107-21-1', kd: '99.5%', cpc: 'SDS PDF', status: 'Verified'},
                                     {kw: 'Propylene Oxide', vol: '75-56-9', kd: '99.9%', cpc: 'COA Scan', status: 'Verified'},
                                     {kw: 'Methanol Tech', vol: '67-56-1', kd: '99.8%', cpc: 'Invoice', status: 'Verified'},
                                     {kw: 'Acetone HPLC', vol: '67-64-1', kd: '99.99%', cpc: 'TDS PDF', status: 'Processing'},
                                     {kw: 'Toluene Nitration', vol: '108-88-3', kd: '99.7%', cpc: 'SDS PDF', status: 'Verified'}
                                 ] as item}
                                 <div class="px-4 py-3 flex items-center hover:bg-gray-50 transition-colors">
                                     <div class="w-1/3 font-medium text-gray-900">{item.kw}</div>
                                     <div class="w-1/6 text-right text-gray-600">{item.vol}</div>
                                     <div class="w-1/6 text-right">
                                         <span class="px-1.5 py-0.5 rounded text-[10px] font-bold bg-green-100 text-green-700">{item.kd}</span>
                                     </div>
                                     <div class="w-1/6 text-right text-gray-600">{item.cpc}</div>
                                     <div class="w-1/6 text-right">
                                         <span class="text-[10px] font-bold {item.status === 'Verified' ? 'text-green-600' : 'text-yellow-600'}">{item.status}</span>
                                     </div>
                                 </div>
                                 {/each}
                            </div>
                        </div>
                    </div>
                 </div>
             </div>
        </div>
        
        <!-- Bottom Grid of 3 items -->
        <div class="grid md:grid-cols-3 gap-0 mt-0 border-x border-b border-gray-200 divide-x divide-gray-200 bg-white">
            <div class="p-6 flex items-start gap-4 hover:bg-gray-50 transition-colors cursor-pointer">
                <div class="w-6 h-6 rounded-full border border-gray-300 flex-shrink-0 flex items-center justify-center text-xs font-mono">1</div>
                <p class="text-xs text-gray-600 leading-relaxed">Extract data from any chemical document format—SDS, COA, TDS, or invoices—with zero manual entry.</p>
            </div>
            <div class="p-6 flex items-start gap-4 hover:bg-gray-50 transition-colors cursor-pointer">
                <div class="w-6 h-6 rounded-full border border-gray-300 flex-shrink-0 flex items-center justify-center text-xs font-mono">2</div>
                <p class="text-xs text-gray-600 leading-relaxed">Cross-reference extracted data against global regulatory databases and manufacturer specifications automatically.</p>
            </div>
            <div class="p-6 flex items-start gap-4 hover:bg-gray-50 transition-colors cursor-pointer">
                <div class="w-6 h-6 rounded-full border border-gray-300 flex-shrink-0 flex items-center justify-center text-xs font-mono">3</div>
                <p class="text-xs text-gray-600 leading-relaxed">Sync verified records directly to your SAP, Oracle, or custom ERP systems via our enterprise-grade API.</p>
            </div>
        </div>
    </div>
</section>