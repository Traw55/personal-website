<script lang="ts">
    import Button from "$lib/components/ui/button/button.svelte";
    import ResumeCard from "$lib/components/ResumeCard.svelte";
    import Title from "$lib/components/Title.svelte";
    import Container from "$lib/components/Container.svelte";
</script>

<svelte:head>
	<title>
		Traw - Resume
	</title>
</svelte:head>

<Container>
    <Title title="Resume" />
    <div class="pt-16 flex flex-col gap-8">
        <div class="flex justify-between items-center">
            <span class="text-2xl font-bold"> Edcation </span>
        </div>
        <ResumeCard
            date="2023 - present"
            title="Software Engineering Bachelor"
            company=" Umm Al-Qura University"
        />
        <div class="flex justify-between items-center"></div>
    </div>
</Container>
