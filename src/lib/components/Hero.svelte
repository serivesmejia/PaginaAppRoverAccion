<script lang="ts">
  import { onMount } from 'svelte';

  const titleLines = ["Conecta.", "Desarrolla.", "Impacta."];
  let typedLines = $state(["", "", ""]);
  let currentLine = $state(0);
  let showCursor = $state(true);

  onMount(() => {
    let charIndex = 0;

    const typeNextChar = () => {
      if (currentLine >= titleLines.length) return;
      
      if (charIndex < titleLines[currentLine].length) {
        typedLines[currentLine] += titleLines[currentLine].charAt(charIndex);
        charIndex++;
        setTimeout(typeNextChar, 80); // Velocidad de escritura del título
      } else {
        currentLine++;
        charIndex = 0;
        setTimeout(typeNextChar, 300); // Pausa breve entre palabras
      }
    };

    setTimeout(typeNextChar, 400); // Esperar un poco antes de empezar

    // Parpadeo del cursor
    setInterval(() => {
      showCursor = !showCursor;
    }, 500);
  });
</script>

<main class="flex flex-col items-center text-center mt-10 md:mt-20">
  <h1 class="text-5xl md:text-7xl font-mono font-black text-[#0B212D] mb-6 uppercase tracking-tight min-h-[160px] md:min-h-[250px] drop-shadow-sm">
    <span class="block">
      {typedLines[0]}
      {#if currentLine === 0}
        <span class={showCursor ? 'opacity-100 text-[#5D4D73]' : 'opacity-0'}>_</span>
      {/if}
    </span>
    <span class="block text-[#5D4D73]">
      {typedLines[1]}
      {#if currentLine === 1}
        <span class={showCursor ? 'opacity-100 text-[#5D4D73]' : 'opacity-0'}>_</span>
      {/if}
    </span>
    <span class="block">
      {typedLines[2]}
      {#if currentLine >= 2}
        <span class={showCursor ? 'opacity-100 text-[#5D4D73]' : 'opacity-0'}>_</span>
      {/if}
    </span>
  </h1>
  
  <p class="text-lg md:text-xl max-w-2xl text-[#2A3B45] font-semibold mb-10 leading-relaxed font-sans animate-fade-in-up" style="animation-delay: 2.2s; animation-fill-mode: both;">
    Una plataforma móvil enfocada en la centralización de proyectos sociales. Fortalece el trabajo colaborativo y escala el impacto de cada iniciativa en la comunidad Scout/Rover.
  </p>
  
  <div class="flex gap-4 flex-wrap justify-center animate-fade-in-up" style="animation-delay: 2.5s; animation-fill-mode: both;">
    <a href="#download" class="bg-[#0B212D] text-white font-mono font-bold px-8 py-4 uppercase tracking-widest hover:bg-[#5D4D73] transition-all cursor-pointer rounded-lg shadow-lg hover:shadow-xl hover:-translate-y-1">
      Descargar APK
    </a>
    <a href="#about" class="bg-white border-2 border-[#0B212D] text-[#0B212D] font-mono font-bold px-8 py-4 uppercase tracking-widest hover:bg-[#F4EBE1] transition-all cursor-pointer rounded-lg shadow-sm hover:shadow-md hover:-translate-y-1">
      Saber Más
    </a>
  </div>
</main>

<style>
  @keyframes fadeInUp {
    from {
      opacity: 0;
      transform: translateY(20px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }
  .animate-fade-in-up {
    animation: fadeInUp 0.8s ease-out forwards;
  }
</style>
