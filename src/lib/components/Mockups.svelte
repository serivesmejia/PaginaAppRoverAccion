<script>
  import img1 from '$lib/assets/1.png';
  import img2 from '$lib/assets/2.png';
  import img3 from '$lib/assets/3.png';
</script>

<section class="grid grid-cols-1 md:grid-cols-3 gap-6 my-10" id="about">
  <div class="border border-[#DABBA1] bg-white h-96 flex items-center justify-center relative group overflow-hidden rounded-xl shadow-sm hover:shadow-md transition-shadow">
    <div class="absolute inset-0 bg-[#37616A]/10 opacity-0 group-hover:opacity-100 transition-opacity z-10 pointer-events-none"></div>
    <img src={img1} alt="Directorio Principal" class="w-full h-full object-contain group-hover:scale-105 transition-transform duration-500" />
  </div>
  <div class="border border-[#DABBA1] bg-white h-96 flex items-center justify-center relative group md:-translate-y-8 overflow-hidden rounded-xl shadow-sm hover:shadow-md transition-shadow">
    <div class="absolute inset-0 bg-[#37616A]/10 opacity-0 group-hover:opacity-100 transition-opacity z-10 pointer-events-none"></div>
    <img src={img2} alt="Lista Proyectos" class="w-full h-full object-contain group-hover:scale-105 transition-transform duration-500" />
  </div>
  <div class="border border-[#DABBA1] bg-white h-96 flex items-center justify-center relative group overflow-hidden rounded-xl shadow-sm hover:shadow-md transition-shadow">
    <div class="absolute inset-0 bg-[#37616A]/10 opacity-0 group-hover:opacity-100 transition-opacity z-10 pointer-events-none"></div>
    <img src={img3} alt="Detalles Proyecto" class="w-full h-full object-contain group-hover:scale-105 transition-transform duration-500" />
  </div>
</section>
