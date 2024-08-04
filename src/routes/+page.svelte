<script lang="ts">
	import Button from "$lib/components/ui/button/button.svelte";
</script>

<div class="flex justify-end">
	<div
		class="bg-secondary text-secondary-foreground relative w-full lg:w-[60vw] h-[40vh] min-h-[calc(100vh-6.5rem)] flex justify-cente items-centerr"
	>
		<div
			class="bg-[#f4ece6] dark:bg-[#303030] shadow-[0_10px_60px_-15px_rgba(0,0,0,0.7)]
           w-[22rem] absolute lg:start-10 lg:-translate-x-full translate-y-1/4
          flex flex-col items-center justify-between pt-8 gap-2 self-start"
		>
			<img
				src="/profile.jpg"
				class="rounded-full w-64 mx-auto grayscale"
				alt="الصورة الشخصية"
			/>
			<div class="flex flex-col items-center gap-8">
				<h1 class="font-bold text-4xl">Traw</h1>
				<hr class="w-24 border-2 border-primary" />
				<h2>Wev Developer</h2>
			</div>

			<div
				class="bg-secondary text-secondary-foreground w-full flex justify-center p-2 mt-12"
			>
				<Button variant="ghost" size="icon"
					><svg
						class="h-auto w-6"
						xmlns="http://www.w3.org/2000/svg"
						viewBox="0 0 24 24"
						><path
							fill="none"
							stroke="currentColor"
							stroke-linecap="round"
							stroke-linejoin="round"
							stroke-width="1.5"
							d="M17 2h-3a5 5 0 0 0-5 5v3H6v4h3v8h4v-8h3l1-4h-4V7a1 1 0 0 1 1-1h3z"
						/></svg
					></Button
				>
				<Button variant="ghost" size="icon"
					><svg
						class="h-auto w-6"
						xmlns="http://www.w3.org/2000/svg"
						viewBox="0 0 16 16"
						><path
							fill="currentColor"
							d="M9.294 6.928L14.357 1h-1.2L8.762 6.147L5.25 1H1.2l5.31 7.784L1.2 15h1.2l4.642-5.436L10.751 15h4.05zM7.651 8.852l-.538-.775L2.832 1.91h1.843l3.454 4.977l.538.775l4.491 6.47h-1.843z"
						/></svg
					></Button
				>
				<Button variant="ghost" size="icon">
					<svg
						class="h-auto w-6"
						xmlns="http://www.w3.org/2000/svg"
						viewBox="0 0 448 512"
						><path
							fill="currentColor"
							d="M416 32H31.9C14.3 32 0 46.5 0 64.3v383.4C0 465.5 14.3 480 31.9 480H416c17.6 0 32-14.5 32-32.3V64.3c0-17.8-14.4-32.3-32-32.3M135.4 416H69V202.2h66.5V416zm-33.2-243c-21.3 0-38.5-17.3-38.5-38.5S80.9 96 102.2 96c21.2 0 38.5 17.3 38.5 38.5c0 21.3-17.2 38.5-38.5 38.5m282.1 243h-66.4V312c0-24.8-.5-56.7-34.5-56.7c-34.6 0-39.9 27-39.9 54.9V416h-66.4V202.2h63.7v29.2h.9c8.9-16.8 30.6-34.5 62.9-34.5c67.2 0 79.7 44.3 79.7 101.9z"
						/></svg
					>
				</Button>
				<Button variant="ghost" size="icon"
					><svg
						class="h-auto w-6"
						xmlns="http://www.w3.org/2000/svg"
						viewBox="0 0 48 48"
						><g fill="none"
							><path
								stroke="currentColor"
								stroke-linejoin="round"
								stroke-width="4"
								d="M34 6H14a8 8 0 0 0-8 8v20a8 8 0 0 0 8 8h20a8 8 0 0 0 8-8V14a8 8 0 0 0-8-8Z"
							/><path
								stroke="currentColor"
								stroke-linejoin="round"
								stroke-width="4"
								d="M24 32a8 8 0 1 0 0-16a8 8 0 0 0 0 16Z"
							/><path
								fill="currentColor"
								d="M35 15a2 2 0 1 0 0-4a2 2 0 0 0 0 4"
							/></g
						></svg
					></Button
				>
			</div>
		</div>
		<div class="ms-10 max-w-[30rem] flex flex-col gap-8 ">
			<h1 class="text-8xl font-extrabold">Hello</h1>
			<h4 class="text-4xl">Here's who I am & what I do</h4>
			<div class="flex gap-2">
				<Button class="w-32">Resume</Button>
				<Button variant="outline" class="w-32">Projects</Button>
			</div>
			<div class="flex flex-col ga-2">
				<p>
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugiat,
					numquam ducimus adipisci dolorem sapiente porro, dolore unde illum
					ipsum nobis accusamus odio! Magnam blanditiis voluptas, provident illo
					autem nesciunt quidem?
				</p>
				<p>
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Architecto
					provident iste incidunt accusantium aliquam debitis dolores, voluptate
					repudiandae libero nam ullam enim in molestias sed pariatur quod
					repellendus neque ea!
				</p>
			</div>
		</div>
	</div>
</div>
