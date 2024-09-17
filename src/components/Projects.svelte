<script>
	import ProjectTemplate from './ProjectTemplate.svelte';

	let projects = [
		{
			title: 'Tin',
			imageUrl:
				'https://user-images.githubusercontent.com/12881812/161390756-f98deb3b-ccb1-495d-bccc-56a2cdeaac99.png',
			altText: 'Code snippet of the Tin language',
			itemUrl: 'https://github.com/The-Tin-Foil-Hat-Society/tin',
			description:
				'Tin is a structured, imperative, and procedural programming language desgined around the RISC-V architecture, aimed at embedded applications.',
			badgeList: ['Flex', 'Bison', 'C', 'RISC-V', 'Python']
		},
		{
			title: 'GAN-Aimbot',
			imageUrl: 'https://raw.githubusercontent.com/kazaxc/GAN-Aimbot/main/Classified.png',
			altText: 'Screenshot of the aimbot identifying targets',
			itemUrl: 'https://github.com/kazaxc/GAN-Aimbot',
			description:
				'GAN-Aimbot is a machine learning Aimbot for the First Person Shooter game CS:GO, making use of the YOLOv8 image classifier it is designed to be easily retrained on any First Person Shooter.',
			badgeList: ['Python', 'YOLOv8', 'Computer Vision', 'Machine Learning']
		},
		{
			title: 'Dotfiles',
			imageUrl: 'https://raw.githubusercontent.com/kazaxc/dotfiles/main/Pictures/dotfiles.png',
			altText: 'Screenshot of desktop configured',
			itemUrl: 'https://github.com/kazaxc/dotfiles',
			description:
				'My dotfiles contain all of the configuration files needed for my Arch Linux setup, including instructions on how to install them. The setup makes use of DWM for window management on XOrg and config for fastfetch, cava and more.',
			badgeList: ['Linux', 'Arch', 'DWM', 'Configuration']
		},
		{
			title: 'LPEngine',
			imageUrl: 'https://raw.githubusercontent.com/kazaxc/LPEngine/main/Cropped.png',
			altText: 'Screenshot of example render',
			itemUrl: 'https://github.com/The-Tin-Foil-Hat-Society/tin',
			description:
				'Testing game engine written in C++ with a Vulkan renderer, the purpose of the engine was to test the performance impact of GameObjects vs ECS and was created as a part of my 4th year project at university.',
			badgeList: ['C++', 'Vulkan', 'ECS']
		},
		{
			title: 'Unity PCG Tool',
			imageUrl:
				'https://user-images.githubusercontent.com/12881812/161390756-f98deb3b-ccb1-495d-bccc-56a2cdeaac99.png',
			altText: 'Screenshot of tool generating some meshes',
			itemUrl: 'https://github.com/The-Tin-Foil-Hat-Society/tin',
			description:
				'Procedural content generation tool for the Unity game engine created to solve a set of unit tests as outlined in a university assignment.',
			badgeList: ['Unity', 'C#', 'PCG', 'Unit Testing']
		},
		{
			title: 'The Jungle',
			imageUrl: 'https://raw.githubusercontent.com/kazaxc/portfolio/main/static/croppedJungle.png',
			altText: 'Gameplay screenshot of a level in the game',
			itemUrl: 'https://github.com/The-Tin-Foil-Hat-Society/tin',
			description:
				'2D platformer game created in the Unity game engine created in an exercise to create a fully fledged polished game from start to finish including art, sfx, music, etc.',
			badgeList: ['Unity', 'C#', '2D', 'Platformer']
		},
		{
			title: 'Tin: Reforged (Coming Soon)',
			imageUrl:
				'https://user-images.githubusercontent.com/12881812/161390756-f98deb3b-ccb1-495d-bccc-56a2cdeaac99.png',
			altText: 'Code snippet of the Tin language',
			itemUrl: 'https://github.com/The-Tin-Foil-Hat-Society/tin',
			description:
				'Tin: Reforged is the sequel to Tin designed to take the core aspects and design of the language and rewrite it in the LLVM compiler infrastructure so that it can be used on a wider range of hardware and be more applicable. Not yet available coming soon!',
			badgeList: ['Flex', 'Bison', 'C', 'Compiler']
		},
		{
			title: 'Panther (Coming Soon)',
			imageUrl: '#',
			altText: 'Image of a rendered scene',
			itemUrl: '#',
			description:
				'Panther will be a game engine written in C++ making use of Vulkan for rendering. The engine will focus on high performance rendering and cutting away bloat that is seen in modern engines. Currently work in progress, repo coming soon!',
			badgeList: ['Flex', 'Bison', 'C', 'Compiler']
		},
		{
			title: 'Craftify',
			imageUrl: '#',
			altText: 'Screenshot of craftify client',
			itemUrl: '#',
			description:
				'Music streaming for the ComputerCraft mod with servers and a custom graphical client. Music is stored ingame in a custom format serialized and sent over a network to a client where the music can be listend to and what is playing managed, inspired by music streaming services but brought into a Minecraft mod.',
			badgeList: ['Lua', 'ComputerCraft', 'Networking', 'GUI']
		}
	];
</script>

<div class="grid grid-cols-3 gap-6 m-8 px-32 justify-items-center">
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
