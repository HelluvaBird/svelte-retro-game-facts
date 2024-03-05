<script lang="ts">
	const information = {
		name: 'Sega Mega Drive ',
		released: '1988',
		generation: 'Fourth',
		initialPrice: 189,
		unitsSold: 30.75,
		description:
			"The Sega Mega Drive also know as the Sega Genesis in North America is a 16-bit \
			fourth generation home console developed by Sega. It was Sega's third console \
			and the successor to the Master System. Contributing to the Mega Drive's success was \
			it's library of arcade game ports, popular sports franchises, and the popularity of \
			Sonic the Hedgehog. It was marketed as the cool console for adolescents. Many games contained \
			mature themes and violence which drew quite a bit of legal scrutiny at the time. None the less \
			the Sega Mega Drive remains a popular retro game console to this day."
	};
</script>

<div class="grid grid-cols-12 gap-x-4 gap-y-8 lg:gap-6">
	<div class="col-span-12 lg:col-span-6">
		<p class="max-w-3xl">{information.description}</p>
	</div>
	<div class="col-span-12 lg:col-span-6 max-h-72 lg:max-h-none">
		<img src="images/MD.png" alt="Sega Mega Drive" class="h-full lg:h-auto" />
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
