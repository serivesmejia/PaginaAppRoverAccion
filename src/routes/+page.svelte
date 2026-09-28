<script lang="ts">
  import Header from '$lib/components/Header.svelte';
  import Hero from '$lib/components/Hero.svelte';
  import Mockups from '$lib/components/Mockups.svelte';
  import Features from '$lib/components/Features.svelte';
  import Download from '$lib/components/Download.svelte';
  import Footer from '$lib/components/Footer.svelte';
</script>

<div class="min-h-screen bg-[#0A0A0A] text-[#E5E5E5] font-sans overflow-x-hidden selection:bg-[#00FF00] selection:text-black">
  <!-- Subtle Grid Background -->
  <div class="fixed inset-0 pointer-events-none opacity-20" style="background-image: linear-gradient(#333 1px, transparent 1px), linear-gradient(90deg, #333 1px, transparent 1px); background-size: 40px 40px;"></div>

  <div class="relative max-w-5xl mx-auto px-6 py-12 flex flex-col gap-20 animate-fade-in-up">
    <Header />
    <Hero />
    <div class="stagger-1"><Mockups /></div>
    <div class="stagger-2"><Features /></div>
    <div class="stagger-3"><Download /></div>
    <div class="stagger-4"><Footer /></div>
  </div>
</div>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600&family=IBM+Plex+Mono:wght@400;600&display=swap');
  
  :global(html) {
    scroll-behavior: smooth;
  }
  
  :global(body) {
    font-family: 'Inter', sans-serif;
    background-color: #0A0A0A;
  }
  
  :global(.font-mono) {
    font-family: 'IBM Plex Mono', monospace;
  }

  .animate-fade-in-up {
    animation: fadeInUp 1s ease-out forwards;
  }

  .stagger-1 { animation: fadeInUp 1s ease-out 0.2s both; }
  .stagger-2 { animation: fadeInUp 1s ease-out 0.4s both; }
  .stagger-3 { animation: fadeInUp 1s ease-out 0.6s both; }
  .stagger-4 { animation: fadeInUp 1s ease-out 0.8s both; }

  @keyframes fadeInUp {
    from {
      opacity: 0;
      transform: translateY(30px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }
</style>
