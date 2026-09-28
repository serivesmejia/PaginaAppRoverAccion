<script>
  import favicon from '$lib/assets/favicon.png';
</script>

<header class="flex justify-between items-center border-b border-[#333] pb-4">
  <div class="flex items-center gap-3">
    <img src={favicon} alt="Logo" class="w-8 h-8 object-contain" />
    <div class="font-mono text-xl text-white font-bold tracking-widest uppercase">
      RoverAcción
    </div>
  </div>
  <nav class="hidden md:flex gap-6 font-mono text-sm">
    <a href="#about" class="hover:text-[#00FF00] transition-colors">[ El_Proyecto ]</a>
    <a href="#features" class="hover:text-[#00FF00] transition-colors">[ Funciones ]</a>
    <a href="#download" class="hover:text-[#00FF00] transition-colors">[ Descargar ]</a>
  </nav>
</header>
