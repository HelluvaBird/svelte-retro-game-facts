<script lang="ts">
	import { page } from '$app/stores';
</script>

<div class="py-32">
	<div class="grid place-items-center">
		<div>
			<h2 class="text-lg text-sky-400">{$page.status}</h2>
			<p>Nothing here but us chickens</p>
			<div class="flex gap-2 my-16">
				<img
					src="images/Chicken.gif"
					alt="Chicken"
					class="w-[160px] h-[170px] [image-rendering:pixelated] mx-auto"
				/>
				<img
					src="images/Chicken.gif"
					alt="Chicken"
					class="w-[160px] h-[170px] [image-rendering:pixelated] mx-auto -scale-x-100"
				/>
				<img
					src="images/Chicken.gif"
					alt="Chicken"
					class="w-[160px] h-[170px] [image-rendering:pixelated] mx-auto"
				/>
			</div>
			<a href="/" class="text-sky-400">Go back home</a>
		</div>
	</div>
</div>
