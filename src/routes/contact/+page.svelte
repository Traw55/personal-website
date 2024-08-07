<script>
    import Container from "$lib/components/Container.svelte";
    import Title from "$lib/components/Title.svelte";
    import  Input  from "$lib/components/ui/input/input.svelte";
    import  Label  from "$lib/components/ui/label/label.svelte";
    import  Textarea from "$lib/components/ui/textarea/textarea.svelte";
    import Button from "$lib/components/ui/button/button.svelte";

</script>

<svelte:head>
	<title>
		Traw - Let's Talk
	</title>
</svelte:head>

<Container class="flex flex-col gap-16">
    <Title title="Let's Talk" />
    <form
    action="https://formsubmit.co/traw547@gmail.com"
    method="post"
     class="bg-secondary text-secondary-foreground p-8 flex flex-col gap-8">
        <div>
            <Label for="name">Full Name</Label>
            <Input required name="name" id="name" placeholder="write your name"/>
        </div>
        <div>
            <Label for="email">Email</Label>
            <Input required type="email" name="email" id="email" placeholder="example@xyz.com"/>
        </div>
        <div>
            <Label for="name">Subject</Label>
            <Input required name="name" id="name" placeholder="write your name"/>
        </div>
        <div>
            <Label for="email">message</Label>
            <Textarea required name="message" id="message" placeholder="..."/>
        </div>
        <Button type="submit" class="max-w-32">
            SEND
        </Button>
    </form>
</Container>