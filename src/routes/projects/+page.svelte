<script lang="ts">
    import Title from "$lib/components/Title.svelte";
    import Container from "$lib/components/Container.svelte";
    import ProjectCard from "$lib/components/ProjectCard.svelte";
    import Button from "$lib/components/ui/button/button.svelte";
</script>

<svelte:head>
	<title>
		Traw - Projects
	</title>
</svelte:head>

<Container class=" flex flex-col gap-16">
    <Title title="Project" />
    <p class="font-bold">
        My project:
    </p>
    <ProjectCard title="Simple Calculator" 
    subtitle="A simple calculator for performing calculator" imageSrc="/project1.png">
    <Button class=" dark:bg-white mb-2 w-32"  href="https://luminous-chimera-ac6c78.netlify.app/">Try it!</Button>
    </ProjectCard>
    <ProjectCard title="To-Do-List" subtitle="A task tracker that helps organize your time and is easy to use"
     imageSrc="/project3.jpg">
       <Button class=" dark:bg-white w-32" href="https://todolisttraw.netlify.app/">Try it!</Button>
    </ProjectCard>
</Container>
