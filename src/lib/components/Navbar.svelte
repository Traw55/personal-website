<script>
    import { page } from "$app/stores";
    import { text } from "@sveltejs/kit";
    import Button from "./ui/button/button.svelte";
    import * as Sheet from "$lib/components/ui/sheet";
    import ThemeSwich from "./ThemeSwich.svelte";
    import Title from "./Title.svelte";


    const link = [
        {
        text: 'About me',
        href: '/'
        },
        {
        text: 'Resume',
        href: '/resume'
        },
        {
        text: 'Projects',
        href: '/projects'
        },
        {
        text: 'Contact',
        href: '/contact'
        },
    ]

	let isSheetOpen = false;
</script>

<header class="bg-secondary text-secondary-foreground py-8 px-6">
    <nav
    class="max-w-screen-2xl flex justify-between items-center mx-auto">
    <a href="/" class="flex items-center gap-2">
        
        <div class="flex items-end gap-1">
            <Title title="Traw" class="text-3xl"/>
            <span class="text-2xl uppercase hidden sm:flex"> / web Developer </span>
        </div>
    </a>

    <div class="flex ">
		<ThemeSwich />

		<!-- large screen -->
        <div class="uppercase hidden lg:flex">
            {#each link as link}
            <Button class=" {$page.url.pathname == link.href && 'text-primary'}"
            href={link.href}
            variant="link">{link.text} </Button>
            
            {/each}
        </div>

		<!-- small screen -->
        <Sheet.Root bind:open={isSheetOpen}>
            <Sheet.Trigger class="flex  lg:hidden">
                <Button variant="ghost" size="icon">
                    <svg 
                    class="w-6 h-auto"
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24">
                    <path 
                    fill="currentColor"
                    d="M18 18v2H6v-2zm3-7v2H3v-2zm-3-7v2H6V4z"
                    /></svg>
                </Button>
            </Sheet.Trigger>
            <Sheet.Content class="flex flex-col justify-center">
                {#each link as link}
            <Button class="text-xl {$page.url.pathname == link.href && 'text-primary'}"
            href={link.href}
            variant="link"
			on:click={() => isSheetOpen = false}
			>{link.text} </Button>
            
            {/each}
            </Sheet.Content>
          </Sheet.Root>
    </div>
</nav>

</header>