<script lang="ts">
    import Button from "$lib/components/ui/button/button.svelte";
</script>

<div class="max-w-screen-sm px-4 mx-auto pt-16">
    <h1 class="mx-auto w-fit text-4xl font-bold flex items-center">
        <div class="bg-primary w-5 h-5 me-4"></div>
        <span>Resume</span>
    </h1>
    <div class="pt-16 flex flex-col gap-8">
        <div class="flex justify-between items-center">
            <span>Experience</span>
            <Button>Download CV</Button>
        </div>
        <div class="bg-secondary p-8 shadow-xl flex items-center gap-16">
            <div class="flex flex-col min-w-32">
                <span class="text-primary font-bold">
                    2023  present
                </span>
                <span class="font-bold">
                    Software Engineering Bachelor 
                </span>
                <span>
                    Umm Al-Qura University
                </span>
            </div>
        </div>
    </div>
</div>
