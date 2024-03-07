<script lang="ts">
	const cards = [
		{
			name: 'Nintendo Entertainment System',
			href: '/nes',
			image: 'NES.png'
		},
		{
			name: 'Super Nintendo Entertainment System',
			href: '/snes',
			image: 'SNES.png'
		},
		{
			name: 'Sega Mega Drive',
			href: '/megadrive',
			image: 'MD.png'
		},
		{
			name: 'Nintendo Game Boy',
			href: '/gameboy',
			image: 'GB.png'
		},
		{
			name: 'Nintendo 64',
			href: '/n64',
			image: 'N64.png'
		},
		{
			name: 'Nintendo Game Boy Advance',
			href: '/gba',
			image: 'GBA.png'
		},
		{
			name: 'Nintendo GameCube',
			href: '/gamecube',
			image: 'GCN.png'
		},
		{
			name: 'Sony Playstation',
			href: '/playstation',
			image: 'PS1.png'
		}
	];
</script>

<h2 class=" text-lg font-medium">Please select a console:</h2>

<div class="mt-24">
	<div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-x-8 gap-y-12 sm:gap-y-8">
		{#each cards as card}
			<div class="relative bg-zinc-800 rounded-lg overflow-hidden">
				<div class="relative h-48 w-full overflow-hidden rounded-lg z-10">
					<img src={`images/${card.image}`} alt="Nintendo Entertainment System" />
				</div>
				<h3 class="text-lg font-medium py-8 px-4 mx-auto sm:max-w-64">
					<a href={card.href}>
						<span class="absolute inset-0 z-10"></span>
						{card.name}
					</a>
				</h3>
				<div class="absolute top-0 inset-x-0 h-48 overflow-hidden">
					<div class="absolute bottom-0 inset-x-0 h-24 bg-gradient-to-t from-zinc-900"></div>
				</div>
			</div>
		{/each}
	</div>
</div>
