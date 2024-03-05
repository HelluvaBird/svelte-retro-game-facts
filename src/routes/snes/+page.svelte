<script lang="ts">
	const information = {
		name: 'Super Nintendo Entertainment System',
		released: '1990',
		generation: 'Fourth',
		initialPrice: 199,
		unitsSold: 49.1,
		description:
			'The Super Nintendo Entertainment System is a 16-bit home video game console \
			 developed by Nintendo that was released in 1990. The console introduced advanced \
			 graphics and sound capabilities compared with other systems at the time. It was \
			 designed to accommodate the ongoing development of a variety of enhancement chips \
			 integrated into game cartridges to be more competitive into the next generation. \
			 The SNES continues to be popular today among collectors, retaining its title as the \
			 best-selling console of the 16-bit generation.'
	};
</script>

<div class="grid grid-cols-12 gap-x-4 gap-y-8 lg:gap-6">
	<div class="col-span-12 lg:col-span-6">
		<p class="max-w-3xl">{information.description}</p>
	</div>
	<div class="col-span-12 lg:col-span-6">
		<img src="images/SNES.png" alt="Super Nintendo Entertainment System" />
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
