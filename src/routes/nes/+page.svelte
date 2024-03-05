<script lang="ts">
	const information = {
		name: 'Nintendo Entertainment System',
		released: '1983',
		discontinued: '1995',
		generation: 'Third',
		initialPrice: 179,
		unitsSold: 61910000,
		description:
			'The Nintendo Entertainment System (NES) is an 8-bit third-generation \
			 home video game console produced by Nintendo. It was first released \
			 in Japan in 1983 as the Family Computer (FC) commonly referred to as Famicom. \
			 It would be redesigned as the NES, and released in American markets on October 18, 1985.\
			 The NES is one of the best-selling consoles of its time and helped revitalize the US gaming \
			 industry following the video game crash of 1983. The NES features several groundbreaking \
			 games, such as Super Mario Brothers, Donkey Kong, The Legend of Zelda, and Metroid. \
			 Many have claimed the NES to be the greatest video game console of all time.'
	};
</script>

<div class="grid grid-cols-12 gap-x-4 gap-y-8 lg:gap-6">
	<div class="col-span-12 lg:col-span-6">
		<p class="max-w-3xl">{information.description}</p>
	</div>
	<div class="col-span-12 lg:col-span-6">
		<img src="images/NES.png" alt="Nintendo Entertainment System" />
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
				<dt class="text-zinc-300 text-base leading-7">Discontinued</dt>
				<dd class="text-zinc-50 text-3xl font-semibold tracking-tight">
					{information.discontinued}
				</dd>
			</div>
		</dl>
	</div>
</div>
