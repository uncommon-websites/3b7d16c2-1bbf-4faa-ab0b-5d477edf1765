<script lang="ts">
  import { onMount } from 'svelte';
  
  let isScrolled = $state(false);

  onMount(() => {
    const handleScroll = () => {
      isScrolled = window.scrollY > 0;
    };
    window.addEventListener('scroll', handleScroll);
    return () => window.removeEventListener('scroll', handleScroll);
  });
</script>

<div class="fixed top-0 w-full z-50 flex flex-col font-sans">
  <!-- Top Announcement Bar -->
  <div class="bg-[#faffb7] py-2 px-4 text-center text-[10px] sm:text-xs font-medium tracking-wide text-gray-900 flex justify-center items-center gap-2">
    <span>🚀 Introducing the Three-Layer AI Architecture: Verified Chemical Data Records</span>
    <a href="#" class="bg-white px-2 py-0.5 rounded text-[10px] font-bold uppercase tracking-wide border border-transparent hover:border-gray-200 transition-colors flex items-center gap-1">
        Learn More 
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-2.5 h-2.5">
            <path stroke-linecap="round" stroke-linejoin="round" d="M13.5 4.5L21 12m0 0l-7.5 7.5M21 12H3" />
        </svg>
    </a>
  </div>

  <!-- Main Nav -->
  <nav class="bg-white/95 backdrop-blur-sm border-b border-gray-100 transition-all duration-200 {isScrolled ? 'py-3' : 'py-4'}">
    <div class="max-w-[1400px] mx-auto px-6 flex items-center justify-between">
      <!-- Logo & Links -->
      <div class="flex items-center gap-10">
        <a href="/" class="text-3xl font-bold tracking-tighter text-black">
          solvate
        </a>
        
        <!-- Desktop Links -->
        <div class="hidden lg:flex items-center gap-8 text-[15px] font-medium text-gray-800">
          <a href="#" class="hover:text-black">Technology</a>
          <a href="#" class="hover:text-black">Compliance</a>
          <a href="#" class="hover:text-black">Case Studies</a>
          <a href="#" class="hover:text-black">Enterprise</a>
        </div>
      </div>

      <!-- Right Actions -->
      <div class="flex items-center gap-6">
        <a href="#" class="text-[15px] font-medium text-gray-800 hover:text-black hidden sm:block">Log In</a>
        <a href="#" class="bg-gray-100 hover:bg-gray-200 text-gray-900 px-5 py-2.5 rounded text-[15px] font-medium transition-colors hidden sm:block">Get Started</a>
        <a href="#" class="bg-[#00ff66] hover:bg-[#00e05a] text-black px-5 py-2.5 rounded-full text-[15px] font-medium transition-colors flex items-center gap-1 shadow-sm">
          Book a Demo
          <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-4 h-4">
            <path stroke-linecap="round" stroke-linejoin="round" d="M13.5 4.5L21 12m0 0l-7.5 7.5M21 12H3" />
          </svg>
        </a>
      </div>
    </div>
  </nav>
</div>
