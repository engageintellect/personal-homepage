<script lang="ts">
	export let pageData = {
		title: 'Josh Chadwick',
		content:
			'Nostrud mollit cupidatat labore aute eu  deserunt et cupidatat cupidatat nostrud qui irure do amet. Duis cupidatat minim culpa cupidatat nulla nisi commodo.',
		image:
			'https://images.unsplash.com/photo-1633356122544-f134324a6cee?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2670&q=80',
		alt: 'hero image',
		primaryBtn: {
			label: 'Learn More',
			link: '/'
		},

		secondaryBtnLeft: {
			label: 'Blog',
			link: 'https://personal-blog-xi-ten.vercel.app/'
		},

		secondaryBtnRight: {
			label: 'Docs',
			link: 'https://engageintellect-docs.vercel.app/'
		}
	};
</script>

<div
	class="hero h-[100vh] lg:h-[45rem] shadow-lg"
	style="background-image: url('https://images.unsplash.com/photo-1633356122544-f134324a6cee?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2670&q=80');"
>
	<div class="hero-overlay bg-opacity-90 bg-neutral-900" />
	<div class="hero-content text-neutral-content">
		<div class="z-60 drop-shadow-lg text-center">
			<div class="mb-5 text-5xl md:text-8xl font-semibold">{pageData.title}</div>
			<div class="mb-5 max-w-md mx-auto">
				{pageData.content}
			</div>
			<div class="flex md:flex-row flex-col gap-4 justify-center">
				<a
					href={pageData.secondaryBtnLeft.link}
					class="btn btn-info transition-color duration-300 text-lg"
				>
					{pageData.secondaryBtnLeft.label}
				</a>

				<a
					href={pageData.primaryBtn.link}
					class="btn btn-primary transition-color duration-300 text-lg"
				>
					{pageData.primaryBtn.label}
				</a>

				<a
					href={pageData.secondaryBtnRight.link}
					class="btn btn-info btn-primary transition-color duration-300 text-lg"
				>
					{pageData.secondaryBtnRight.label}
				</a>
			</div>
		</div>
	</div>
</div>
