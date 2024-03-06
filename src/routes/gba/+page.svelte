<script lang="ts">
	const information = {
		name: 'Nintendo Game Boy Advance',
		released: '2001',
		generation: 'Sixth',
		initialPrice: 99.99,
		unitsSold: 81.51,
		description:
			"The Game Boy Advance is a 32-bit sixth generation handheld game console \
		developed by Nintendo. The Game Boy Advance was praised for it's graphical capabilities, \
		battery life, and backwards compatibility with Game Boy cartridges. The lack of a back-lit \
		screen was often mentioned as a drawback. Later iterations of the Game Boy Advance would \
		address this issue. Some Game Boy Advance games had special built-in features including \
		rumble features, tilt sensors, and solar sensors. Many games were also ported to the Game \
		Boy Advance from previous 8-bit and 16-bit generations"
	};
</script>

<div class="grid grid-cols-12 gap-x-4 gap-y-8 lg:gap-6">
	<div class="col-span-12 lg:col-span-6">
		<p class="max-w-3xl">{information.description}</p>
	</div>
	<div class="col-span-12 lg:col-span-6 justify-self-center max-h-72">
		<img src="images/GBA.png" alt="Nintendo Game Boy Advance" class="h-full" />
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
