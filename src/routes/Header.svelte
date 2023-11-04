<script>
	import { toggleMode, mode } from 'mode-watcher'
	import { Button } from '$lib/components/ui/button'
	import '../app.postcss'
	// import { Sun, Moon, Instagram } from 'lucide-svelte'
	import {
		Sun,
		Moon,
		DiscordLogo,
		InstagramLogo,
		GithubLogo,
		CaretRight,
		ArrowRight,
		Calendar,
	} from 'radix-icons-svelte'

	let theme_mode = ''
	mode.subscribe((m) => (theme_mode = m))
</script>

<header class="flex align-center justify-center p-6">
	<nav class="flex justify-between items-center">
		<!-- left section -->
		<a href="/">
			<!-- change logo dark/light mode -->
			<img
				src={theme_mode == 'dark' ? 'dark.svg' : 'light.svg'}
				id="logo"
				alt="Logo"
				class="w-52 h-auto"
			/>
		</a>

		<!-- middle section -->
		<ul class="flex justify-evenly items-center font-medium space-x-7">
			<li><a href="/discover">Discover</a></li>
			<li><a href="/discover">Events</a></li>
			<li><a href="/resources">Resources</a></li>
			<li><a href="/pathways">About Us</a></li>
			<!-- <li class='flex items-center'>
				<a href="/contact">Contact</a>
				<CaretRight class="h-[1.5rem] w-[1.5rem]"/>
			</li> -->
		</ul>

		<!-- right section -->
		<div class="rounded-md w-52 pl-2 flex justify-between items-center">
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
			<a class="icon" href="https://github.com">
				<GithubLogo
				class="h-[1.5rem] w-[1.5rem] rotate-0 scale-100 transition-all"
				/>
			</a>
			<a class="icon" href="https://www.calendar.google.com">
				<Calendar
					class="h-[1.5rem] w-[1.5rem] rotate-0 scale-100 transition-all"
				/>
			</a>
			<Button on:click={toggleMode} variant="outline" size="icon">
				<Sun
					class="h-[1.5rem] w-[1.5rem] rotate-0 scale-100 transition-all dark:-rotate-90 dark:scale-0"
				/>
				<Moon
					class="absolute h-[1.5rem] w-[1.5rem] rotate-90 scale-0 transition-all dark:rotate-0 dark:scale-100"
				/>
				<span class="sr-only">Toggle theme</span>
			</Button>
		</div>
	</nav>
</header>

<style>
	nav {
		width: clamp(50rem, 100%, 68rem);
	}
</style>
