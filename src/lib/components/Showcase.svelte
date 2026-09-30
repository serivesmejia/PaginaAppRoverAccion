<section class="w-full bg-[#143E50] rounded-xl shadow-lg p-10 flex flex-col md:flex-row items-center justify-between gap-8 relative overflow-hidden">
  <!-- Accent corners -->
  <div class="absolute top-0 right-0 w-12 h-12 border-t-4 border-r-4 border-[#DABBA1] rounded-tr-xl opacity-50"></div>
  <div class="absolute bottom-0 left-0 w-12 h-12 border-b-4 border-l-4 border-[#DABBA1] rounded-bl-xl opacity-50"></div>

  <div class="md:w-2/3 z-10">
    <h2 class="text-3xl font-mono text-white font-bold uppercase mb-4">De Rovers para Rovers</h2>
    <p class="text-[#F4EBE1]/90 text-sm leading-relaxed mb-4">
      RoverAcción nació de la necesidad real de conectar nuestras propias iniciativas dentro de la red. Entendemos perfectamente lo difícil que es encontrar voluntarios y hacer que los proyectos sociales trasciendan más allá de nuestros clanes.
    </p>
    <p class="text-[#F4EBE1]/70 text-sm leading-relaxed">
      Esta plataforma fue diseñada pensando en las necesidades específicas de nuestra comunidad, integrando validación por CUM, historiales de voluntariado y trabajo alineado a los Objetivos de Desarrollo Sostenible (ODS) de la ONU.
    </p>
  </div>
  
  <div class="md:w-1/3 flex justify-center z-10">
    <div class="w-32 h-32 rounded-full border-4 border-[#37616A] bg-[#0B212D] flex items-center justify-center shadow-inner relative">
      <div class="absolute inset-2 border-2 border-dashed border-[#5D4D73] rounded-full animate-spin-slow"></div>
      <svg class="w-12 h-12 text-[#CEE8E2]" fill="currentColor" viewBox="0 0 24 24">
        <!-- Ícono de estrella/logro scout -->
        <path d="M12 2L15.09 8.26L22 9.27L17 14.14L18.18 21.02L12 17.77L5.82 21.02L7 14.14L2 9.27L8.91 8.26L12 2Z" />
      </svg>
    </div>
  </div>
</section>

<style>
  .animate-spin-slow {
    animation: spin 15s linear infinite;
  }
  @keyframes spin {
    from { transform: rotate(0deg); }
    to { transform: rotate(360deg); }
  }
</style>
