<script>
  let activeTab = 'Production';
  const tabs = ['Production', 'Quality', 'Maintenance', 'Logistics'];
</script>

<section class="py-24 bg-white text-center">
  <div class="max-w-[1200px] mx-auto px-6">
    <h2 class="text-5xl font-bold mb-6 tracking-tight text-gray-900">
      Real-Time<br>Collaboration
    </h2>
    
    <!-- Tabs -->
    <div class="flex justify-center mb-8">
      <div class="bg-gray-100 p-1 rounded-lg inline-flex">
        {#each tabs as tab}
          <button 
            class="px-4 py-1.5 text-sm font-medium rounded-md transition-all {activeTab === tab ? 'bg-white text-gray-900 shadow-sm' : 'text-gray-500 hover:text-gray-700'}"
            on:click={() => activeTab = tab}
          >
            {tab}
          </button>
        {/each}
      </div>
    </div>

    <p class="text-lg text-gray-600 mb-16 max-w-2xl mx-auto leading-relaxed">
      Work together seamlessly across shifts and departments.<br>
      Share updates, flag issues, and keep operations running smoothly.
    </p>

    <!-- UI Mockup -->
    <div class="bg-white rounded-xl shadow-2xl overflow-hidden border border-gray-200 text-left h-[700px] flex flex-col">
      <!-- Toolbar -->
      <div class="h-12 border-b border-gray-200 flex items-center justify-between px-4 bg-white">
        <div class="flex items-center gap-4">
           <span class="text-xs font-mono text-gray-500">WF-2024-0147</span>
           <span class="text-gray-300">/</span>
           <span class="text-xs font-bold text-gray-900 flex items-center gap-2">
             <span class="w-2 h-2 rounded-full bg-green-500"></span>
             Assembly Line 3 - Active
           </span>
        </div>
        
        <div class="flex items-center gap-6">
           <div class="flex items-center gap-4 text-xs font-medium text-gray-500">
              <button class="hover:text-gray-900 flex items-center gap-1"><span>👁️</span> Overview</button>
              <button class="text-red-500 flex items-center gap-1 border-b-2 border-red-500 pb-3 mt-3"><span>💬</span> Updates <span class="bg-red-100 text-red-600 px-1 rounded text-[10px]">5</span></button>
              <button class="hover:text-gray-900 flex items-center gap-1"><span>📊</span> Metrics</button>
           </div>
        </div>

        <div class="flex items-center gap-2">
           <button class="text-xs border border-gray-200 rounded px-2 py-1 flex items-center gap-1 text-gray-600">Filter ▼</button>
           <button class="text-xs border border-gray-200 rounded px-2 py-1 flex items-center gap-1 text-gray-600">Export ▼</button>
        </div>
      </div>

      <div class="flex flex-1 overflow-hidden">
        <!-- Left Sidebar (Stations) -->
        <div class="w-64 bg-gray-50 border-r border-gray-200 flex flex-col text-xs">
           <div class="p-2 border-b border-gray-200 flex items-center justify-between">
              <span class="font-bold text-gray-700">STATIONS</span>
              <div class="flex gap-1 text-gray-400">
                 <span>🔍</span>
                 <span>⚙️</span>
              </div>
           </div>
           <div class="flex-1 overflow-y-auto p-2 space-y-1">
              <div class="flex items-center gap-2 text-gray-600 pl-2">
                 <span>▼</span> <span>Receiving</span> <span class="ml-auto text-[10px] bg-green-100 text-green-600 px-1 rounded">Active</span>
              </div>
              <div class="flex items-center gap-2 text-gray-600 pl-2">
                 <span>▼</span> <span>Pre-Assembly</span> <span class="ml-auto text-[10px] bg-green-100 text-green-600 px-1 rounded">Active</span>
              </div>
              <div class="flex items-center gap-2 font-medium text-gray-900 pl-2 bg-blue-50 rounded py-1">
                 <span>▼</span> <span>Assembly Line 3</span> <span class="ml-auto text-[10px] bg-green-100 text-green-600 px-1 rounded">Active</span>
              </div>
              <div class="pl-6 space-y-1">
                 <div class="flex items-center gap-2 text-gray-700">
                    <span>●</span> <span>Station 3A</span> <span class="ml-auto text-[10px] bg-yellow-100 text-yellow-700 px-1 rounded">Busy</span>
                 </div>
                 <div class="flex items-center gap-2 text-gray-700">
                    <span>●</span> <span>Station 3B</span> <span class="ml-auto text-[10px] bg-green-100 text-green-600 px-1 rounded">Ready</span>
                 </div>
                 <div class="flex items-center gap-2 text-gray-500">
                    <span>●</span> <span>Station 3C</span> <span class="ml-auto text-[10px] bg-yellow-100 text-yellow-700 px-1 rounded">Busy</span>
                 </div>
                 <div class="flex items-center gap-2 text-gray-500">
                    <span>●</span> <span>Station 3D</span> <span class="ml-auto text-[10px] bg-green-100 text-green-600 px-1 rounded">Ready</span>
                 </div>
                 <div class="flex items-center gap-2 text-gray-500">
                    <span>●</span> <span>Station 3E</span> <span class="ml-auto text-[10px] bg-red-100 text-red-600 px-1 rounded">Issue</span>
                 </div>
              </div>
              <div class="flex items-center gap-2 text-gray-600 pl-2 pt-2">
                 <span>▶</span> <span>Quality Control</span> <span class="ml-auto text-[10px] bg-green-100 text-green-600 px-1 rounded">Active</span>
              </div>
           </div>
        </div>

        <!-- Center (Floor View) -->
        <div class="flex-1 bg-gray-100 relative flex items-center justify-center overflow-hidden">
           <!-- Floor layout visualization -->
           <div class="w-[500px] h-[400px] bg-white rounded-xl shadow-inner relative p-8">
              <!-- Production line visualization -->
              <div class="flex items-center justify-between h-full">
                 <!-- Station boxes -->
                 <div class="flex flex-col items-center gap-2">
                    <div class="w-20 h-20 bg-yellow-100 border-2 border-yellow-400 rounded-lg flex items-center justify-center">
                       <span class="text-xs font-bold text-yellow-700">3A</span>
                    </div>
                    <span class="text-[10px] text-gray-600">Busy</span>
                 </div>
                 
                 <div class="flex-1 h-0.5 bg-gray-300 mx-2"></div>
                 
                 <div class="flex flex-col items-center gap-2">
                    <div class="w-20 h-20 bg-green-100 border-2 border-green-400 rounded-lg flex items-center justify-center">
                       <span class="text-xs font-bold text-green-700">3B</span>
                    </div>
                    <span class="text-[10px] text-gray-600">Ready</span>
                 </div>
                 
                 <div class="flex-1 h-0.5 bg-gray-300 mx-2"></div>
                 
                 <div class="flex flex-col items-center gap-2">
                    <div class="w-20 h-20 bg-yellow-100 border-2 border-yellow-400 rounded-lg flex items-center justify-center">
                       <span class="text-xs font-bold text-yellow-700">3C</span>
                    </div>
                    <span class="text-[10px] text-gray-600">Busy</span>
                 </div>
                 
                 <div class="flex-1 h-0.5 bg-gray-300 mx-2"></div>
                 
                 <div class="flex flex-col items-center gap-2 relative">
                    <div class="w-20 h-20 bg-red-100 border-2 border-red-400 rounded-lg flex items-center justify-center">
                       <span class="text-xs font-bold text-red-700">3E</span>
                    </div>
                    <span class="text-[10px] text-gray-600">Issue</span>
                    <!-- Alert Pin -->
                    <div class="absolute -top-2 -right-2 w-6 h-6 bg-red-500 rounded-full border-2 border-white shadow-lg flex items-center justify-center text-white font-bold text-xs cursor-pointer z-10 hover:scale-110 transition-transform">
                       !
                    </div>
                 </div>
              </div>
           </div>
           
           <!-- Overlay controls -->
           <div class="absolute bottom-4 left-1/2 transform -translate-x-1/2 bg-white rounded-full shadow-lg px-4 py-2 flex gap-4 text-gray-500 text-xs">
              <button>Refresh</button>
              <button>|</button>
              <button>Layout</button>
           </div>
           
           <!-- User Avatars overlay -->
           <div class="absolute top-4 left-1/2 transform -translate-x-1/2 bg-white/80 backdrop-blur rounded-full px-3 py-1 flex items-center gap-2 text-xs shadow-sm">
              <div class="flex -space-x-2">
                 <div class="w-6 h-6 rounded-full bg-blue-500 border-2 border-white"></div>
                 <div class="w-6 h-6 rounded-full bg-green-500 border-2 border-white"></div>
                 <div class="w-6 h-6 rounded-full bg-yellow-500 border-2 border-white"></div>
              </div>
              <span class="text-gray-600">4 operators online</span>
           </div>
        </div>

        <!-- Right Sidebar (Comments) -->
        <div class="w-80 bg-white border-l border-gray-200 flex flex-col">
           <div class="p-4 border-b border-gray-100">
              <div class="flex items-center gap-2 mb-3">
                 <div class="w-6 h-6 rounded-full bg-gray-200"></div>
                 <input type="text" placeholder="Add a comment..." class="flex-1 bg-transparent text-sm focus:outline-none">
              </div>
              <div class="flex justify-between items-center">
                 <div class="flex gap-2 text-gray-400">
                    <button>📎</button>
                    <button>@</button>
                    <button>😊</button>
                 </div>
                 <button class="bg-blue-500 text-white text-xs px-3 py-1.5 rounded font-medium">Post</button>
              </div>
           </div>
           
           <div class="flex-1 overflow-y-auto p-4 space-y-6">
              <div class="flex items-center justify-between text-[10px] font-bold text-gray-400 uppercase tracking-wider mb-2">
                 <span>All Comments</span>
                 <div class="flex gap-2">
                    <button>Filter</button>
                    <button>Sort</button>
                 </div>
              </div>

              <!-- Comment 1 -->
              <div class="flex gap-3">
                 <div class="w-8 h-8 rounded-full bg-blue-100 flex-shrink-0"></div>
                 <div>
                    <div class="flex items-baseline gap-2 mb-1">
                       <span class="text-xs font-bold text-gray-900">Maria Santos</span>
                       <span class="text-[10px] text-gray-400">12m</span>
                    </div>
                    <div class="text-xs text-gray-600 bg-gray-50 p-2 rounded-lg border border-gray-100 mb-1">
                       <span class="text-blue-500">@team</span> Station 3E sensor malfunction resolved. Back online in 5 minutes.
                    </div>
                    <div class="flex items-center gap-2 mt-1">
                       <div class="w-4 h-4 rounded-full bg-gray-200"></div>
                       <span class="text-[10px] text-gray-400">Add a reply...</span>
                    </div>
                 </div>
              </div>

              <!-- Comment 2 -->
              <div class="flex gap-3 relative">
                 <div class="absolute -left-2 top-2 w-1 h-12 bg-gray-100 rounded-full"></div> <!-- Thread line -->
                 <div class="w-8 h-8 rounded-full bg-red-100 flex-shrink-0 z-10"></div>
                 <div>
                    <div class="flex items-baseline gap-2 mb-1">
                       <span class="text-xs font-bold text-gray-900">James Park</span>
                       <span class="text-[10px] text-gray-400">18m</span>
                    </div>
                    <div class="text-xs text-gray-600 mb-1">
                       Station 3E showing error code E-47. Need maintenance check ASAP.
                    </div>
                    <div class="flex items-center gap-2 mt-1">
                       <div class="w-4 h-4 rounded-full bg-gray-200"></div>
                       <span class="text-[10px] text-gray-400">Add a reply...</span>
                    </div>
                 </div>
              </div>
           </div>
        </div>
      </div>
    </div>
  </div>
</section>
