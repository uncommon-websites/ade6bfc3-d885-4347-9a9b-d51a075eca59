<script>
</script>

<section class="bg-[#0B0F19] text-white py-24">
  <div class="max-w-[1200px] mx-auto px-6">
    <div class="text-center mb-16">
      <h2 class="text-5xl font-bold mb-6 tracking-tight">
        Intelligent Task Orchestration
      </h2>
      <p class="text-gray-400 text-lg max-w-2xl mx-auto leading-relaxed">
        Stop chasing down status updates. Company automatically routes tasks, tracks progress, and keeps everyone aligned—turning chaos into coordinated action.
      </p>
    </div>

    <!-- Task Dashboard UI Mockup -->
    <div class="bg-white rounded-lg overflow-hidden shadow-2xl mb-20 text-gray-900 mx-auto max-w-[1000px]">
      <!-- Window Header -->
      <div class="bg-gray-50 border-b border-gray-200 px-4 py-2 flex items-center justify-between">
         <div class="flex items-center gap-2">
            <span class="text-xs font-semibold text-gray-700">Production Floor - Shift A</span>
         </div>
         <div class="flex items-center gap-3">
            <div class="flex items-center gap-1 text-xs text-gray-500 bg-white border border-gray-200 px-2 py-1 rounded">
               <span>👁️</span> Live View
            </div>
            <div class="flex items-center gap-1 text-xs text-gray-500 bg-white border border-gray-200 px-2 py-1 rounded">
               <span>📊</span> Analytics
            </div>
            <div class="flex items-center gap-1 text-xs text-gray-500 bg-white border border-gray-200 px-2 py-1 rounded">
               <span>⬇️</span> Export
            </div>
            <button class="text-gray-400 hover:text-gray-600">✕</button>
         </div>
      </div>

      <!-- Table Header -->
      <div class="grid grid-cols-12 bg-gray-50 border-b border-gray-200 text-[10px] font-bold text-gray-500 uppercase tracking-wider py-2 px-4">
         <div class="col-span-1">Status</div>
         <div class="col-span-1">Priority</div>
         <div class="col-span-3">Task Name</div>
         <div class="col-span-2">Assigned To</div>
         <div class="col-span-2">Station</div>
         <div class="col-span-1">Progress</div>
         <div class="col-span-1">Due</div>
         <div class="col-span-1">Actions</div>
      </div>

      <!-- Table Body - Live Tasks -->
      <div class="h-[400px] bg-white relative">
         <!-- Search Overlay Effect -->
         <div class="absolute top-4 left-4 right-4 bg-white border border-gray-200 shadow-sm rounded p-2 flex items-center gap-2 max-w-md z-10">
            <span class="text-gray-400">🔍</span>
            <span class="text-sm text-gray-900">Filter tasks|</span>
            <div class="w-[1px] h-4 bg-[oklch(0.546_0.245_262.881)] animate-pulse"></div>
         </div>
         
         <!-- Blurred/Faded rows to simulate content behind search -->
         <div class="opacity-30 pointer-events-none">
             {#each Array(8) as _, i}
             <div class="grid grid-cols-12 border-b border-gray-100 py-3 px-4 text-xs text-gray-600">
                <div class="col-span-1 flex items-center"><div class="w-2 h-2 rounded-full bg-green-500 mr-2"></div> Active</div>
                <div class="col-span-1"><span class="text-orange-600">●</span> High</div>
                <div class="col-span-3">Quality Inspection #{i + 1}</div>
                <div class="col-span-2">Operator {i + 1}</div>
                <div class="col-span-2">Station {Math.floor(Math.random() * 5) + 1}</div>
                <div class="col-span-1">{Math.floor(Math.random() * 100)}%</div>
                <div class="col-span-1">2h</div>
                <div class="col-span-1">...</div>
             </div>
             {/each}
         </div>
      </div>
    </div>

    <!-- Features Grid -->
    <div class="grid grid-cols-1 md:grid-cols-3 gap-x-12 gap-y-16 text-left">
       <!-- Feature 1 -->
       <div>
          <div class="flex items-center gap-3 mb-3">
             <div class="text-gray-400">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 2v20M2 12h20"/></svg>
             </div>
             <h3 class="text-lg font-bold text-white">Smart Task Routing</h3>
          </div>
          <p class="text-sm text-gray-400 leading-relaxed">
             Tasks automatically route to the right person based on skills, availability, and workload. No more manual assignments.
          </p>
       </div>

       <!-- Feature 2 -->
       <div>
          <div class="flex items-center gap-3 mb-3">
             <div class="text-gray-400">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="10"/><polyline points="12 6 12 12 16 14"/></svg>
             </div>
             <h3 class="text-lg font-bold text-white">Real-Time Progress</h3>
          </div>
          <p class="text-sm text-gray-400 leading-relaxed">
             See exactly where every task stands. Live updates eliminate status meetings and keep everyone informed.
          </p>
       </div>

       <!-- Feature 3 -->
       <div>
          <div class="flex items-center gap-3 mb-3">
             <div class="text-gray-400">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"/><polyline points="22 4 12 14.01 9 11.01"/></svg>
             </div>
             <h3 class="text-lg font-bold text-white">Automated Handoffs</h3>
          </div>
          <p class="text-sm text-gray-400 leading-relaxed">
             When one step completes, the next begins automatically. Smooth transitions between shifts and stations.
          </p>
       </div>

       <!-- Feature 4 -->
       <div>
          <div class="flex items-center gap-3 mb-3">
             <div class="text-gray-400">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M10.29 3.86L1.82 18a2 2 0 0 0 1.71 3h16.94a2 2 0 0 0 1.71-3L13.71 3.86a2 2 0 0 0-3.42 0z"/><line x1="12" y1="9" x2="12" y2="13"/><line x1="12" y1="17" x2="12.01" y2="17"/></svg>
             </div>
             <h3 class="text-lg font-bold text-white">Exception Alerts</h3>
          </div>
          <p class="text-sm text-gray-400 leading-relaxed">
             Get notified instantly when tasks stall or deadlines approach. Proactive alerts prevent small issues from becoming big problems.
          </p>
       </div>

       <!-- Feature 5 -->
       <div>
          <div class="flex items-center gap-3 mb-3">
             <div class="text-gray-400">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="22 12 18 12 15 21 9 3 6 12 2 12"/></svg>
             </div>
             <h3 class="text-lg font-bold text-white">Performance Analytics</h3>
          </div>
          <p class="text-sm text-gray-400 leading-relaxed">
             Track cycle times, bottlenecks, and throughput. Data-driven insights help you optimize operations continuously.
          </p>
       </div>

       <!-- Feature 6 -->
       <div>
          <div class="flex items-center gap-3 mb-3">
             <div class="text-gray-400">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/><path d="M23 21v-2a4 4 0 0 0-3-3.87"/><path d="M16 3.13a4 4 0 0 1 0 7.75"/></svg>
             </div>
             <h3 class="text-lg font-bold text-white">Team Coordination</h3>
          </div>
          <p class="text-sm text-gray-400 leading-relaxed">
             Everyone sees what they need to do next. Clear priorities and dependencies keep teams moving in sync.
          </p>
       </div>
    </div>
  </div>
</section>
