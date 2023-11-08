<script>
	import '../app.postcss'
	// import { Sun, Moon, Instagram } from 'lucide-svelte'
	import {
		DiscordLogo,
		InstagramLogo,
		GithubLogo,
		CaretRight,
		ArrowRight,
		Calendar,
		HamburgerMenu,
		Link2,
	} from 'radix-icons-svelte'
</script>

<!-- <header
	class="flex items-center justify-center p-6 border-green-500 box-border border-b-4 h-[10vh]"
> -->
<header class="flex items-center justify-center p-6 h-[10vh]">
	<nav class="flex justify-between items-center">
		<!-- left section -->
		<a href="/">
			<!-- change logo dark/light mode -->
			<img
				src="dark_career-catalysts_v2.svg"
				id="logo"
				alt="Logo"
				class="w-auto h-16"
			/>
		</a>

		<!-- middle section -->
		<ul
			class="flex justify-evenly items-center font-medium space-x-7 min-w-[25rem]"
		>
			<li><a href="/discover">Discover</a></li>
			<li><a href="/events">Events</a></li>
			<li><a href="/resources">Resources</a></li>
			<li><a href="/about_us">About Us</a></li>
			<!-- <li class='flex items-center'>
				<a href="/contact">Contact</a>
				<CaretRight class="h-[1.5rem] w-[1.5rem]"/>
			</li> -->
		</ul>

		<!-- right section -->
		<div
			id="right"
			class="rounded-md w-52 pl-2 flex justify-between items-center"
		>
			<a class="icon" href="https://www.instagram.com/careercatalystclub/">
				<InstagramLogo
					class="h-[1.5rem] w-[1.5rem] rotate-0 scale-100 transition-all"
				/>
			</a>
			<a class="icon" href="https://discord.gg/3UU4YQar">
				<DiscordLogo
					class="h-[1.5rem] w-[1.5rem] rotate-0 scale-100 transition-all"
				/>
			</a>
			<a class="icon" href="https://github.com/Career-Catalysts">
				<GithubLogo
					class="h-[1.5rem] w-[1.5rem] rotate-0 scale-100 transition-all"
				/>
			</a>
			<a class="icon" href="https://www.calendar.google.com">
				<Calendar
					class="h-[1.5rem] w-[1.5rem] rotate-0 scale-100 transition-all"
				/>
			</a>
			<a class="linktree" href="https://linktr.ee/CareerCatalysts">
				<Link2
					class="h-[1.5rem] w-[1.5rem] rotate-0 scale-100 transition-all"
				/>
			</a>
			<!-- <Button on:click={toggleMode} variant="outline" size="icon">
				<Sun
					class="h-[1.5rem] w-[1.5rem] rotate-0 scale-100 transition-all dark:-rotate-90 dark:scale-0"
				/>
				<Moon
					class="absolute h-[1.5rem] w-[1.5rem] rotate-90 scale-0 transition-all dark:rotate-0 dark:scale-100"
				/>
				<span class="sr-only">Toggle theme</span>
			</Button> -->
		</div>
	</nav>
</header>

<style>
	nav {
		width: clamp(50rem, 100%, 68rem);
	}

	@media (width < 900px) {
		.icon {
			display: none;
		}
		#right {
			justify-content: end;
		}
	}
</style>
