<div class="relative bg-black rounded-[3rem] p-3 w-full h-full shadow-2xl ring-1 ring-gray-900/5">
  <!-- Power Button -->
  <div class="absolute -right-[2px] top-24 w-[2px] h-12 bg-gray-800 rounded-r-md"></div>
  <!-- Volume Buttons -->
  <div class="absolute -left-[2px] top-24 w-[2px] h-8 bg-gray-800 rounded-l-md"></div>
  <div class="absolute -left-[2px] top-36 w-[2px] h-8 bg-gray-800 rounded-l-md"></div>

  <!-- Screen -->
  <div class="bg-white w-full h-full rounded-[2.5rem] overflow-hidden relative flex flex-col">
    <!-- Status Bar / Notch Area -->
    <div class="h-12 w-full flex justify-center items-start pt-2 absolute top-0 left-0 z-20">
      <div class="w-28 h-7 bg-black rounded-full flex items-center justify-center gap-2 px-3">
        <!-- Dynamic Island Content Simulation -->
        <div class="w-full h-full flex items-center justify-between opacity-0">
           <!-- Hidden content just to keep size -->
        </div>
      </div>
    </div>

    <!-- App Content -->
    <div class="flex-1 overflow-y-auto pt-12 px-6 pb-6 text-xs font-medium select-none scrollbar-hide">
      <!-- Header -->
      <div class="flex justify-between items-baseline mb-6 mt-2">
        <h2 class="text-3xl font-bold tracking-tight">Mon<span class="text-red-500 ml-0.5">•</span></h2>
        <div class="text-gray-400 text-[10px] uppercase tracking-wide text-right leading-tight font-semibold">
          December 9<br>2024
        </div>
      </div>

      <!-- Calendar Strip -->
      <div class="flex justify-between mb-8 text-[10px] text-gray-400 font-semibold">
        <div class="flex flex-col items-center gap-1.5">
          <span class="w-7 h-7 rounded-full bg-black text-white flex items-center justify-center font-bold text-xs">9</span>
          <span class="text-black font-bold tracking-wide">MON</span>
        </div>
        <div class="flex flex-col items-center gap-1.5 opacity-50">
          <span class="h-7 flex items-center justify-center text-xs">10</span>
          <span class="tracking-wide">TUE</span>
        </div>
        <div class="flex flex-col items-center gap-1.5 opacity-50">
          <span class="h-7 flex items-center justify-center text-xs">11</span>
          <span class="tracking-wide">WED</span>
        </div>
        <div class="flex flex-col items-center gap-1.5 opacity-50">
          <span class="h-7 flex items-center justify-center text-xs">12</span>
          <span class="tracking-wide">THU</span>
        </div>
        <div class="flex flex-col items-center gap-1.5 opacity-50">
          <span class="h-7 flex items-center justify-center text-xs">13</span>
          <span class="tracking-wide">FRI</span>
        </div>
        <div class="flex flex-col items-center gap-1.5 opacity-50">
          <span class="h-7 flex items-center justify-center text-xs">14</span>
          <span class="tracking-wide">SAT</span>
        </div>
        <div class="flex flex-col items-center gap-1.5 opacity-50">
          <span class="h-7 flex items-center justify-center text-xs">15</span>
          <span class="tracking-wide">SUN</span>
        </div>
      </div>

      <!-- List -->
      <div class="space-y-5">
        <!-- Item 1 -->
        <div class="flex items-center gap-4">
          <span class="text-red-500 text-lg leading-none">✻</span>
          <span class="font-semibold text-sm">Daria's 20th Birthday</span>
        </div>

        <!-- Item 2 -->
        <div class="flex items-center gap-4 justify-between group">
          <div class="flex items-center gap-4">
            <span class="text-yellow-500 text-lg leading-none">☀</span>
            <span class="text-sm font-medium">Wake up</span>
          </div>
          <span class="text-gray-300 font-medium">09:00</span>
        </div>

        <!-- Item 3 -->
        <div class="flex items-center gap-4 justify-between">
          <div class="flex items-center gap-4">
            <span class="text-gray-400 border border-gray-300 rounded-[4px] w-5 h-5 flex items-center justify-center text-[9px] font-serif italic">Aa</span>
            <span class="text-sm font-medium">Design Crit</span>
          </div>
          <span class="text-gray-300 font-medium">10:00</span>
        </div>

        <!-- Item 4 -->
        <div class="flex items-center gap-4 justify-between">
          <div class="flex items-center gap-4">
            <span class="text-gray-400 border border-gray-300 rounded-[4px] w-5 h-5 flex items-center justify-center text-[10px] -rotate-90">✂</span>
            <span class="text-sm font-medium">Haircut with Vincent</span>
          </div>
          <span class="text-gray-300 font-medium">13:00</span>
        </div>

        <!-- Item 5 -->
        <div class="flex items-center gap-4">
          <span class="text-black border-[1.5px] border-black rounded-full w-5 h-5 flex items-center justify-center text-[10px] font-bold">✓</span>
          <span class="text-sm font-medium line-through text-gray-400">Make pasta</span>
        </div>

        <!-- Item 6 -->
        <div class="flex items-center gap-4 text-gray-400">
          <span class="border-[1.5px] border-dashed border-gray-300 rounded-full w-5 h-5"></span>
          <span class="text-sm font-medium">Pushups x100</span>
        </div>

        <!-- Item 7 -->
        <div class="flex items-center gap-4 justify-between text-gray-400">
          <div class="flex items-center gap-4">
            <span class="text-purple-400 text-lg leading-none">☾</span>
            <span class="text-black text-sm font-medium">Wind down</span>
          </div>
          <span class="text-gray-300 font-medium">21:00</span>
        </div>
      </div>
    </div>
    
    <!-- Home Indicator -->
    <div class="absolute bottom-1 left-1/2 -translate-x-1/2 w-32 h-1 bg-black rounded-full opacity-20"></div>
  </div>
</div>

