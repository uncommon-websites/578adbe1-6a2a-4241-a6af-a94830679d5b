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
      <div class="flex justify-between items-center mb-6 mt-2">
        <h2 class="text-2xl font-bold tracking-tight">123 Crown St</h2>
        <div class="w-8 h-8 rounded-full bg-gray-900 text-white flex items-center justify-center text-xs font-bold">
          SC
        </div>
      </div>

      <!-- Rent Card -->
      <div class="bg-gradient-to-br from-gray-50 to-gray-100 rounded-2xl p-4 mb-6 border border-gray-200">
        <div class="flex justify-between items-start mb-3">
          <div>
            <div class="text-[10px] text-gray-500 uppercase tracking-wide font-semibold mb-1">Next Rent Due</div>
            <div class="text-2xl font-bold">$2,800</div>
          </div>
          <div class="text-right">
            <div class="text-[10px] text-gray-500 uppercase tracking-wide font-semibold mb-1">Due Date</div>
            <div class="text-sm font-bold">Jan 15</div>
          </div>
        </div>
        <div class="text-[10px] text-gray-600 font-medium">Your share: $700</div>
      </div>

      <!-- Housemates Section -->
      <div class="mb-6">
        <h3 class="text-[10px] text-gray-500 uppercase tracking-wide font-semibold mb-3">Housemates (4)</h3>
        <div class="space-y-2.5">
          <div class="flex items-center justify-between">
            <div class="flex items-center gap-2.5">
              <div class="w-7 h-7 rounded-full bg-gray-900 text-white flex items-center justify-center text-[10px] font-bold">SC</div>
              <span class="text-sm font-medium">Scott (You)</span>
            </div>
            <span class="text-xs text-gray-500 font-medium">$700</span>
          </div>
          <div class="flex items-center justify-between">
            <div class="flex items-center gap-2.5">
              <div class="w-7 h-7 rounded-full bg-gray-200 text-gray-700 flex items-center justify-center text-[10px] font-bold">EM</div>
              <span class="text-sm font-medium">Emma</span>
            </div>
            <span class="text-xs text-gray-500 font-medium">$700</span>
          </div>
          <div class="flex items-center justify-between">
            <div class="flex items-center gap-2.5">
              <div class="w-7 h-7 rounded-full bg-gray-200 text-gray-700 flex items-center justify-center text-[10px] font-bold">JK</div>
              <span class="text-sm font-medium">Jake</span>
            </div>
            <span class="text-xs text-gray-500 font-medium">$700</span>
          </div>
          <div class="flex items-center justify-between">
            <div class="flex items-center gap-2.5">
              <div class="w-7 h-7 rounded-full bg-gray-200 text-gray-700 flex items-center justify-center text-[10px] font-bold">LM</div>
              <span class="text-sm font-medium">Lily</span>
            </div>
            <span class="text-xs text-gray-500 font-medium">$700</span>
          </div>
        </div>
      </div>

      <!-- Bills Section -->
      <div class="mb-6">
        <h3 class="text-[10px] text-gray-500 uppercase tracking-wide font-semibold mb-3">Upcoming Bills</h3>
        <div class="space-y-2.5">
          <div class="flex items-center justify-between">
            <div class="flex items-center gap-2.5">
              <div class="w-5 h-5 rounded bg-yellow-100 flex items-center justify-center text-[10px]">⚡</div>
              <span class="text-sm font-medium">Electricity</span>
            </div>
            <span class="text-xs text-gray-500 font-medium">Jan 20</span>
          </div>
          <div class="flex items-center justify-between">
            <div class="flex items-center gap-2.5">
              <div class="w-5 h-5 rounded bg-blue-100 flex items-center justify-center text-[10px]">📶</div>
              <span class="text-sm font-medium">Internet</span>
            </div>
            <span class="text-xs text-gray-500 font-medium">Jan 25</span>
          </div>
        </div>
      </div>

      <!-- Tasks Section -->
      <div>
        <h3 class="text-[10px] text-gray-500 uppercase tracking-wide font-semibold mb-3">Household Tasks</h3>
        <div class="space-y-2.5">
          <div class="flex items-center gap-2.5">
            <div class="w-5 h-5 rounded-full border-[1.5px] border-black flex items-center justify-center">
              <div class="w-2 h-2 rounded-full bg-black"></div>
            </div>
            <span class="text-sm font-medium">Take out bins</span>
          </div>
          <div class="flex items-center gap-2.5 text-gray-400">
            <div class="w-5 h-5 rounded-full border-[1.5px] border-gray-300"></div>
            <span class="text-sm font-medium">Buy toilet paper</span>
          </div>
        </div>
      </div>
    </div>
    
    <!-- Home Indicator -->
    <div class="absolute bottom-1 left-1/2 -translate-x-1/2 w-32 h-1 bg-black rounded-full opacity-20"></div>
  </div>
</div>

