<script lang="ts">
	const information = {
		name: 'Nintendo 64',
		released: '1996',
		generation: 'Fifth',
		initialPrice: 199.99,
		unitsSold: 32.93,
		description:
			"The Nintendo 64 is a fifth generation home video game console developed by Nintendo. \
		The Nintendo 64 was named after its 64-bit CPU. This CPU aided in the console's 3D capabilities. \
		The console is one of the most widely recognized video game consoles thanks to it's controllers. Due \
		to the competition using CD-ROM based games many third party developers did not develop as many \
		games for the Nintendo 64. Despite this the Nintendo 64 has some of the greatest games ever made \
		including Super Mario 64, The Legend of Zelda: Ocarina of Time, and GoldenEye 007."
	};
</script>

<div class="grid grid-cols-12 gap-x-4 gap-y-8 lg:gap-6">
	<div class="col-span-12 lg:col-span-6">
		<p class="max-w-3xl">{information.description}</p>
	</div>
	<div class="col-span-12 lg:col-span-6 max-h-72 lg:max-h-none">
		<img src="images/N64.png" alt="Super Nintendo Entertainment System" class="h-full lg:h-auto" />
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
