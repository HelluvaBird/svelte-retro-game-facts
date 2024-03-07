<script lang="ts">
	export let title: string | null;

	$: switch (title) {
		case '/':
			title = 'Retro Game Facts';
			break;
		case '/nes':
			title = 'Nintendo Entertainment System';
			break;
		case '/snes':
			title = 'Super Nintendo Entertainment System';
			break;
		case '/megadrive':
			title = 'Sega Mega Drive';
			break;
		case '/gameboy':
			title = 'Nintendo Game Boy';
			break;
		case '/n64':
			title = 'Nintendo 64';
			break;
		case '/gba':
			title = 'Nintendo Game Boy Advance';
			break;
		case '/gamecube':
			title = 'Nintendo GameCube';
			break;
		case '/playstation':
			title = 'Sony Playstation';
			break;
	}
</script>

<header class="bg-sky-950 shadow">
	<div class="max-w-7xl mx-auto py-6 px-4 sm:px-6 lg:px-8">
		<h1 class="text-3xl font-bold tracking-tight">{title}</h1>
	</div>
</header>
