<script>
	export let title;
	export let imageUrl;
	export let altText;
	export let itemUrl;
	export let description;
	export let badgeList = [];
</script>

<a href={itemUrl} class="block h-160">
	<div
		class="card w-full h-full bg-base-100 shadow-xl
      hover:bg-base-200 hover:shadow-2xl
      hover:scale-105 transition-transform duration-300
      px-6"
	>
		<figure class="px-10 pt-10 h-54">
			<img src={imageUrl} alt={altText} class="object-cover w-full h-full rounded-xl" />
		</figure>
		<div class="card-body text-center">
			<h2 class="card-title justify-center">{title}</h2>
			<p>{description}</p>
			<div class="card-actions justify-center">
				{#each badgeList as badge}
					<div class="badge badge-outline">{badge}</div>
				{/each}
			</div>
		</div>
	</div>
</a>
