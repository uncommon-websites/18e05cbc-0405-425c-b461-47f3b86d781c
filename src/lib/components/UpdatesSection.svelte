<section class="py-20 border-b border-border">
	<div class="container-custom">
		<div class="grid grid-cols-1 md:grid-cols-2 gap-16">
			
			<!-- Left Column: CTA & Visual -->
			<div class="flex flex-col h-full">
				<div class="mb-8">
					<p class="font-mono text-xs text-muted mb-4">Start building</p>
					<h2 class="text-2xl font-medium mb-4">Towards a programmatic web for AIs</h2>
					<p class="text-muted font-light mb-8 text-sm leading-relaxed max-w-md">
						Parallel is building new interfaces, infrastructure, and business models for AIs to work with the web
					</p>
					<div class="flex gap-3 mb-12">
						<button class="border border-border px-3 py-1.5 text-xs font-mono uppercase hover:bg-primary-50 transition-colors flex items-center gap-2">
							TRY IT FOR FREE
							<span class="text-muted border border-muted/30 rounded px-1 text-[9px] min-w-[16px] text-center">P</span>
						</button>
						<button class="border border-border px-3 py-1.5 text-xs font-mono uppercase hover:bg-primary-50 transition-colors flex items-center gap-2">
							JOIN US
							<span class="text-muted border border-muted/30 rounded px-1 text-[9px] min-w-[16px] text-center">J</span>
						</button>
					</div>
				</div>
				
				<!-- Barcode Visual -->
				<div class="mt-auto w-full h-48 bg-black relative overflow-hidden flex items-center justify-center">
					{#each Array(100) as _, i}
						<div 
							class="h-full bg-white absolute" 
							style="
								left: {i}%; 
								width: {Math.random() * 2}%; 
								opacity: {Math.random()};
							"
						></div>
					{/each}
					<div class="absolute inset-0 flex items-center justify-center">
						<div class="bg-black text-white font-mono text-[10px] px-2 py-1 z-10">
							parallel.web
						</div>
					</div>
				</div>
			</div>

			<!-- Right Column: Updates -->
			<div>
				<p class="font-mono text-xs text-muted mb-8">Latest updates</p>
				
				<div class="space-y-12">
					<!-- Update 1 -->
					<div class="flex gap-8 group">
						<div class="font-mono text-xs text-muted w-24 shrink-0 pt-1">November 20</div>
						<div>
							<h3 class="font-medium text-sm mb-2 group-hover:text-accent transition-colors cursor-pointer">Introducing Parallel Extract</h3>
							<p class="text-xs text-muted leading-relaxed mb-3">
								Parallel Extract converts web pages into LLM-ready markdown format. It operates in two modes: compressed excerpts (dense, semantically relevant content) and full content extraction (complete page content). The API is designed for AI agents and handles challenging web content including JavaScript-rendered sites and complex PDFs, making it useful for tasks like documentation extraction, research paper processing, and financial filing analysis.
							</p>
							<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Product Release</span>
						</div>
					</div>

					<!-- Update 2 -->
					<div class="flex gap-8 group">
						<div class="font-mono text-xs text-muted w-24 shrink-0 pt-1">November 15</div>
						<div>
							<h3 class="font-medium text-sm mb-2 group-hover:text-accent transition-colors cursor-pointer">Introducing Parallel FindAll</h3>
							<p class="text-xs text-muted leading-relaxed mb-3">
								Parallel's new FindAll API turns natural language queries into custom datasets from the web. It finds entities like companies, people, or locations based on your criteria, then enriches them with structured data—all with citations. FindAll Pro achieves 61% recall, 3x better than competitors.
							</p>
							<div class="flex gap-2">
								<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Product Release</span>
								<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Benchmarks</span>
							</div>
						</div>
					</div>

					<!-- Update 3 -->
					<div class="flex gap-8 group">
						<div class="font-mono text-xs text-muted w-24 shrink-0 pt-1">November 13</div>
						<div>
							<h3 class="font-medium text-sm mb-2 group-hover:text-accent transition-colors cursor-pointer">Introducing Parallel Monitor</h3>
							<p class="text-xs text-muted leading-relaxed mb-3">
								Parallel Monitor can be thought of as a web search that's always on: you define a query that kicks off an ongoing stream of updates every time new related information appears on the web.
							</p>
							<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Product Release</span>
						</div>
					</div>

					<!-- Update 4 -->
					<div class="flex gap-8 group">
						<div class="font-mono text-xs text-muted w-24 shrink-0 pt-1">November 12</div>
						<div>
							<h3 class="font-medium text-sm mb-2 group-hover:text-accent transition-colors cursor-pointer">Parallel raises $100M Series A to build web infrastructure for agents</h3>
							<p class="text-xs text-muted leading-relaxed mb-3">
								Parallel raises $100M Series A at a 740M valuation.
							</p>
							<span class="bg-gray-100 text-[10px] px-1.5 py-0.5 rounded text-muted">Fundraise</span>
						</div>
					</div>
				</div>
			</div>

		</div>
	</div>
</section>
