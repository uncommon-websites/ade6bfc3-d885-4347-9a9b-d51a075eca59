<script>
</script>

<section class="pt-20 pb-16 text-center max-w-[1200px] mx-auto px-6">
  <h1 class="text-6xl font-bold tracking-tight text-gray-900 mb-6 leading-[1.1]">
    Transform Chaos<br>Into Clarity
  </h1>
  <p class="text-lg text-gray-600 mb-8 max-w-2xl mx-auto leading-relaxed">
    Company transforms workflows into automated processes through intelligent task orchestration and real-time data integration. Perfect for operations managers who need control without the documentation chaos.
  </p>
  <button class="bg-[oklch(0.546_0.245_262.881)] text-white px-6 py-3 rounded-lg hover:bg-[oklch(0.488_0.243_264.376)] transition-colors font-semibold text-sm mb-20 cursor-pointer">
    Get started
  </button>

  <!-- Workflow Visualization -->
  <div class="relative w-full aspect-[2/1] bg-gray-50 rounded-xl overflow-hidden flex items-center justify-center border border-gray-100">
    <!-- Abstract workflow representation -->
    <div class="relative w-full h-full flex items-center justify-center p-12">
       <!-- Workflow nodes -->
       <div class="flex items-center gap-8">
          <!-- Start node -->
          <div class="flex flex-col items-center gap-2">
             <div class="w-16 h-16 bg-[oklch(0.546_0.245_262.881)] rounded-full flex items-center justify-center text-white shadow-lg">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                   <circle cx="12" cy="12" r="10"/>
                   <polyline points="12 6 12 12 16 14"/>
                </svg>
             </div>
             <span class="text-xs font-medium text-gray-600">Trigger</span>
          </div>
          
          <!-- Arrow -->
          <div class="flex items-center gap-1">
             <div class="w-12 h-0.5 bg-gray-300"></div>
             <div class="w-0 h-0 border-t-4 border-t-transparent border-b-4 border-b-transparent border-l-8 border-l-gray-300"></div>
          </div>
          
          <!-- Process node -->
          <div class="flex flex-col items-center gap-2">
             <div class="w-16 h-16 bg-gray-800 rounded-lg flex items-center justify-center text-white shadow-lg">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                   <rect x="3" y="3" width="18" height="18" rx="2"/>
                   <path d="M9 9h6M9 15h6"/>
                </svg>
             </div>
             <span class="text-xs font-medium text-gray-600">Process</span>
          </div>
          
          <!-- Arrow -->
          <div class="flex items-center gap-1">
             <div class="w-12 h-0.5 bg-gray-300"></div>
             <div class="w-0 h-0 border-t-4 border-t-transparent border-b-4 border-b-transparent border-l-8 border-l-gray-300"></div>
          </div>
          
          <!-- Decision node -->
          <div class="flex flex-col items-center gap-2">
             <div class="w-16 h-16 bg-yellow-500 rounded-lg rotate-45 flex items-center justify-center text-white shadow-lg">
                <svg class="-rotate-45" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                   <path d="M12 8v8M8 12h8"/>
                </svg>
             </div>
             <span class="text-xs font-medium text-gray-600">Decision</span>
          </div>
          
          <!-- Arrow -->
          <div class="flex items-center gap-1">
             <div class="w-12 h-0.5 bg-gray-300"></div>
             <div class="w-0 h-0 border-t-4 border-t-transparent border-b-4 border-b-transparent border-l-8 border-l-gray-300"></div>
          </div>
          
          <!-- Complete node -->
          <div class="flex flex-col items-center gap-2">
             <div class="w-16 h-16 bg-green-500 rounded-full flex items-center justify-center text-white shadow-lg">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                   <polyline points="20 6 9 17 4 12"/>
                </svg>
             </div>
             <span class="text-xs font-medium text-gray-600">Complete</span>
          </div>
       </div>
    </div>
    
    <div class="absolute inset-0 bg-gradient-to-t from-white via-transparent to-transparent pointer-events-none"></div>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-12 mt-20 text-left">
    <div>
      <div class="text-xs font-semibold text-gray-400 mb-2">01</div>
      <h3 class="text-xl font-bold text-gray-900 mb-2">Visual Workflows</h3>
      <p class="text-sm text-gray-500 leading-relaxed">
        Transform undocumented processes into clear, visual workflows. No coding required—just drag, drop, and automate your operations.
      </p>
    </div>
    <div>
      <div class="text-xs font-semibold text-gray-400 mb-2">02</div>
      <h3 class="text-xl font-bold text-gray-900 mb-2">Real-Time Integration</h3>
      <p class="text-sm text-gray-500 leading-relaxed">
        Connect your existing systems and data sources seamlessly. Keep everything synchronized without manual data entry or spreadsheets.
      </p>
    </div>
    <div>
      <div class="text-xs font-semibold text-gray-400 mb-2">03</div>
      <h3 class="text-xl font-bold text-gray-900 mb-2">Smart Orchestration</h3>
      <p class="text-sm text-gray-500 leading-relaxed">
        Intelligent task routing and automation that learns from your operations. Reduce errors and speed up your manufacturing processes.
      </p>
    </div>
  </div>
</section>
