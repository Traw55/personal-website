<script lang="ts">
    import Button from "$lib/components/ui/button/button.svelte";
    import ResumeCard from "$lib/components/ResumeCard.svelte";
    import Title from "$lib/components/Title.svelte";
    import Container from "$lib/components/Container.svelte";
</script>

<Container>
    <Title title="Resume"/>
    <div class="pt-16 flex flex-col gap-8">
        <div class="flex justify-between items-center">
            <span class="text-2xl font-bold"> Edcation </span>
            <Button>Download CV</Button>
        </div>
        <ResumeCard
            date="2023 - present"
            title="Software Engineering Bachelor"
            company=" Umm Al-Qura University"
        />
        <ResumeCard
            date="2023 - present"
            title="Software Engineering Bachelor"
            company=" Umm Al-Qura University"
        ></ResumeCard>
    </div>
</Container>