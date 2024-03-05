<script lang="ts">
	const information = {
		name: 'Nintendo Game Boy',
		released: '1989',
		generation: 'Fourth',
		initialPrice: 89.99,
		unitsSold: 118.69,
		description:
			"The Game Boy is an 8-bit fourth generation handheld game console developed by \
			Nintendo. Upon the Game Boy's release it was deemed inferior to that of it's \
			fourth generation competition. Despite this the Game Boy outsold the competition \
			and remains one of the best-selling video game consoles of all-time. The Game Boy \
			is seen by many as a cultural icon and one of the most recognizable devices from \
			the 1990's. The Game Boy would introduce a generation to the popular game Tetris as \
			well as the Pokemon franchise years later."
	};
</script>

<div class="grid grid-cols-12 gap-x-4 gap-y-8 lg:gap-6">
	<div class="col-span-12 lg:col-span-6">
		<p class="max-w-3xl">{information.description}</p>
	</div>
	<div class="col-span-12 lg:col-span-6 justify-self-center max-h-72">
		<img src="images/GB.png" alt="Nintendo Game Boy" class="h-full" />
	</div>
	<div class="col-span-12">
		<dl class="grid sm:grid-cols-2 lg:grid-cols-4 gap-x-8 gap-y-12 sm:gap-y-16">
			<div class="flex flex-col-reverse gap-y-3 border-s ps-7 border-zinc-50/20">
				<dt class="text-zinc-300 text-base leading-7">Released</dt>
				<dd class="text-zinc-50 text-3xl font-semibold tracking-tight">{information.released}</dd>
			</div>
			<div class="flex flex-col-reverse gap-y-3 border-s ps-7 border-zinc-50/20">
				<dt class="text-zinc-300 text-base leading-7">Generation</dt>
				<dd class="text-zinc-50 text-3xl font-semibold tracking-tight">{information.generation}</dd>
			</div>
			<div class="flex flex-col-reverse gap-y-3 border-s ps-7 border-zinc-50/20">
				<dt class="text-zinc-300 text-base leading-7">Price</dt>
				<dd class="text-zinc-50 text-3xl font-semibold tracking-tight">
					{information.initialPrice.toLocaleString('en-US', {
						style: 'currency',
						currency: 'USD',
						currencyDisplay: 'symbol'
					})}
				</dd>
			</div>
			<div class="flex flex-col-reverse gap-y-3 border-s ps-7 border-zinc-50/20">
				<dt class="text-zinc-300 text-base leading-7">Sold <span class="text-sm">(units)</span></dt>
				<dd class="text-zinc-50 text-3xl font-semibold tracking-tight">
					{information.unitsSold}M
				</dd>
			</div>
		</dl>
	</div>
</div>
