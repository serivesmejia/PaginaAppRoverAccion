<script>
  import img1 from '$lib/assets/1.png';
  import img2 from '$lib/assets/2.png';
  import img3 from '$lib/assets/3.png';
</script>

<section class="grid grid-cols-1 md:grid-cols-3 gap-8 my-16" id="about">
  <!-- Tarjeta 1: Directorio -->
  <div class="flex flex-col items-center">
    <div class="w-full border border-[#DABBA1] bg-white h-96 flex items-center justify-center relative group overflow-hidden rounded-xl shadow-sm hover:shadow-md transition-shadow mb-4">
      <div class="absolute inset-0 bg-[#37616A]/10 opacity-0 group-hover:opacity-100 transition-opacity z-10 pointer-events-none"></div>
      <img src={img1} alt="Directorio Principal" class="w-full h-full object-contain group-hover:scale-105 transition-transform duration-500" />
    </div>
    <h4 class="font-mono font-bold text-lg text-[#0B212D]">Directorio Dinámico</h4>
    <p class="text-sm text-[#2A3B45] text-center mt-1">Encuentra y contacta a otros miembros de la red.</p>
  </div>

  <!-- Tarjeta 2: Feed Proyectos -->
  <div class="flex flex-col items-center md:-translate-y-8">
    <div class="w-full border border-[#DABBA1] bg-white h-96 flex items-center justify-center relative group overflow-hidden rounded-xl shadow-sm hover:shadow-md transition-shadow mb-4">
      <div class="absolute inset-0 bg-[#37616A]/10 opacity-0 group-hover:opacity-100 transition-opacity z-10 pointer-events-none"></div>
      <img src={img2} alt="Lista Proyectos" class="w-full h-full object-contain group-hover:scale-105 transition-transform duration-500" />
    </div>
    <h4 class="font-mono font-bold text-lg text-[#0B212D]">Feed de Iniciativas</h4>
    <p class="text-sm text-[#2A3B45] text-center mt-1">Explora proyectos activos y los ODS que atienden.</p>
  </div>

  <!-- Tarjeta 3: Detalles -->
  <div class="flex flex-col items-center">
    <div class="w-full border border-[#DABBA1] bg-white h-96 flex items-center justify-center relative group overflow-hidden rounded-xl shadow-sm hover:shadow-md transition-shadow mb-4">
      <div class="absolute inset-0 bg-[#37616A]/10 opacity-0 group-hover:opacity-100 transition-opacity z-10 pointer-events-none"></div>
      <img src={img3} alt="Detalles Proyecto" class="w-full h-full object-contain group-hover:scale-105 transition-transform duration-500" />
    </div>
    <h4 class="font-mono font-bold text-lg text-[#0B212D]">Detalles a Fondo</h4>
    <p class="text-sm text-[#2A3B45] text-center mt-1">Conoce objetivos, planificaciones y súmate como voluntario.</p>
  </div>
</section>
