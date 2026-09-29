<script>
  import favicon from '$lib/assets/favicon.png';
</script>

<header class="flex justify-between items-center border-b border-[#DABBA1] pb-4">
  <div class="flex items-center gap-3">
    <img src={favicon} alt="Logo" class="w-8 h-8 object-contain" />
    <div class="font-mono text-xl text-[#143E50] font-bold tracking-widest uppercase">
      RoverAcción
    </div>
  </div>
  <nav class="hidden md:flex gap-6 font-mono text-sm">
    <a href="#about" class="text-[#143E50] hover:text-[#37616A] transition-colors">[ El_Proyecto ]</a>
    <a href="#features" class="text-[#143E50] hover:text-[#37616A] transition-colors">[ Funciones ]</a>
    <a href="#download" class="text-[#143E50] hover:text-[#37616A] transition-colors">[ Descargar ]</a>
  </nav>
</header>
