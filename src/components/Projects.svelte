<script>
	import ProjectTemplate from './ProjectTemplate.svelte';

	let projects = [
		{
			title: 'Tin',
			imageUrl:
				'https://user-images.githubusercontent.com/12881812/161390756-f98deb3b-ccb1-495d-bccc-56a2cdeaac99.png',
			altText: 'Code snippet of the Tin language',
			itemUrl: 'https://github.com/The-Tin-Foil-Hat-Society/tin',
			description: 'SOME TEST TEXT YAYAYYAYAYAYYAYAYAYAYAYAYAYAYAYAYAYAYAYAY',
			badgeList: ['Flex', 'Bison', 'C', 'Compiler']
		},
		{
			title: 'Tin',
			imageUrl:
				'https://user-images.githubusercontent.com/12881812/161390756-f98deb3b-ccb1-495d-bccc-56a2cdeaac99.png',
			altText: 'Code snippet of the Tin language',
			itemUrl: 'https://github.com/The-Tin-Foil-Hat-Society/tin',
			description: 'SOME TEST TEXT YAYAYYAYAYAYYAYAYAYAYAYAYAYAYAYAYAYAYAYAY',
			badgeList: ['Flex', 'Bison', 'C', 'Compiler']
		},
		{
			title: 'Tin',
			imageUrl:
				'https://user-images.githubusercontent.com/12881812/161390756-f98deb3b-ccb1-495d-bccc-56a2cdeaac99.png',
			altText: 'Code snippet of the Tin language',
			itemUrl: 'https://github.com/The-Tin-Foil-Hat-Society/tin',
			description: 'SOME TEST TEXT YAYAYYAYAYAYYAYAYAYAYAYAYAYAYAYAYAYAYAYAY',
			badgeList: ['Flex', 'Bison', 'C', 'Compiler']
		}
	];
</script>

<div class="grid grid-cols-3 gap-6 m-8">
	{#each projects as project}
		<ProjectTemplate
			title={project.title}
			imageUrl={project.imageUrl}
			altText={project.altText}
			itemUrl={project.itemUrl}
			description={project.description}
			badgeList={project.badgeList}
		/>
	{/each}
</div>
