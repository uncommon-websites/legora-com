<script lang="ts">
  import { onMount } from 'svelte';
  
  let isScrolled = false;

  onMount(() => {
    const handleScroll = () => {
      isScrolled = window.scrollY > 0;
    };
    window.addEventListener('scroll', handleScroll);
    return () => window.removeEventListener('scroll', handleScroll);
  });
</script>

<div class="bg-black text-white text-[11px] py-2 text-center font-sans tracking-wide">
  <span class="opacity-80">News</span> <span class="mx-2 opacity-40">|</span> <span class="font-medium">Legora announces Portal</span> <a href="#" class="ml-1 opacity-80 hover:opacity-100 transition-opacity">Read more →</a>
</div>

<header class="sticky top-0 z-50 bg-white/90 backdrop-blur-sm transition-all duration-300 border-b border-transparent {isScrolled ? 'border-gray-100 py-3' : 'py-5'}">
  <div class="max-w-[1400px] mx-auto px-6 flex items-center justify-between">
    <div class="flex items-center">
      <a href="/" class="text-2xl font-serif tracking-tight">LEGORA</a>
    </div>

    <nav class="hidden md:flex items-center gap-8 text-[13px] font-medium text-gray-600">
      <a href="#" class="hover:text-black transition-colors">Product</a>
      <a href="#" class="hover:text-black transition-colors">Solutions</a>
      <a href="#" class="hover:text-black transition-colors">Security</a>
      <a href="#" class="hover:text-black transition-colors">Customers</a>
      <a href="#" class="hover:text-black transition-colors">News</a>
      <a href="#" class="hover:text-black transition-colors">Careers</a>
      <a href="#" class="hover:text-black transition-colors">Log in</a>
    </nav>
  </div>
</header>
