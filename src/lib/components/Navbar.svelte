<script lang="ts">
	import { page } from '$app/stores';

	const links = [
		{
			title: 'NES',
			href: '/nes'
		},
		{
			title: 'SNES',
			href: '/snes'
		},
		{
			title: 'MD',
			href: '/megadrive'
		},
		{
			title: 'GB',
			href: '/gameboy'
		},
		{
			title: 'N64',
			href: '/n64'
		},
		{
			title: 'GBA',
			href: '/gba'
		},
		{
			title: 'GCN',
			href: '/gamecube'
		},
		{
			title: 'PS1',
			href: '/playstation'
		}
	];
</script>

<nav class="bg-zinc-800">
	<div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
		<div class="flex items-center justify-between h-16">
			<div class="flex items-center">
				<a href="/">
					<svg
						xmlns="http://www.w3.org/2000/svg"
						fill="none"
						viewBox="0 0 24 24"
						stroke-width="1.5"
						stroke="currentColor"
						class="w-8 h-8 stroke-sky-400"
					>
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							d="M8.25 3v1.5M4.5 8.25H3m18 0h-1.5M4.5 12H3m18 0h-1.5m-15 3.75H3m18 0h-1.5M8.25 19.5V21M12 3v1.5m0 15V21m3.75-18v1.5m0 15V21m-9-1.5h10.5a2.25 2.25 0 0 0 2.25-2.25V6.75a2.25 2.25 0 0 0-2.25-2.25H6.75A2.25 2.25 0 0 0 4.5 6.75v10.5a2.25 2.25 0 0 0 2.25 2.25Zm.75-12h9v9h-9v-9Z"
						/>
					</svg>
				</a>
				<div class="hidden md:block">
					<ul class="ms-10 flex items-baseline space-x-4">
						{#each links as link}
							<li>
								<a
									href={link.href}
									class={`px-3 py-2 text-sm font-medium rounded-md ${link.href === $page.route.id ? 'bg-zinc-900 text-zinc-50' : 'text-zinc-200 hover:bg-zinc-700 hover:text-zinc-50'}`}
									>{link.title}</a
								>
							</li>
						{/each}
					</ul>
				</div>
			</div>
		</div>
	</div>
</nav>
