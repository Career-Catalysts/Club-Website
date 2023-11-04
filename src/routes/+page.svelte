<script lang="ts">
	import Button from '$lib/components/ui/button/button.svelte'

	const pauseAnimation = () => {
		const team = document.getElementsByClassName(
			'team'
		) as HTMLCollectionOf<HTMLDivElement>
		for (const t of team) {
			if (t.style) {
				t.style.animationPlayState = 'paused'
			} else {
				console.log('team is null')
			}
		}
	}
</script>

<!-- <div class="max-w-6xl"> -->
<div
  class="flex items-center min-w-[50rem] w-[90%] max-w-[70vw] h-full"
>
  <aside class="flex">
    <section class="flex flex-col justify-center">
      <h1 class="mb-5 max-w-3xl text-7xl font-small">
        Turning Interviews Into Opportunities.
      </h1>
      <h2 class="max-w-xl text-5xl font-semibold">Together We Succeed.</h2>
    </section>
  </aside>


	<aside class="w-[20%]">
		<section>
			<svg viewBox="0 0 500 500">
				<path
					id="outliers"
					pathLength="1"
					stroke="black"
					stroke-width="3"
					fill="none"
					d="M 100 100 l 70 5 l 30 20 l 50 -30 l 50 40 l 50 0 l 30 -20 l 30 10 20 0"
				/>
				<path
					class="team"
					pathLength="1"
					stroke="purple"
					stroke-width="3"
					fill="none"
					d="M 100 200 l 100 0 l 50 15 l 50 0 l 70 -10 l 70 50 l 40 0"
				/>
				<path
					class="team"
					pathLength="1"
					stroke="purple"
					stroke-width="3"
					fill="none"
					d="M 100 250 l 100 0 l 50 -5 l 30 0 l 50 30 l 50 0 l 50 -10 l 50 0"
				/>
				<path
					class="team"
					pathLength="1"
					stroke="purple"
					stroke-width="3"
					fill="none"
					d="M 100 300 l 100 0 l 30 -10 l 50 30 l 70 -20 l 50 0 l 50 -25 l 30 0"
				/>
			</svg>
			<!-- <img src="github.svg" alt="" width="100" height="100" /> -->
		</section>
	</aside>
</div>

<style>
	path {
		stroke-dasharray: 1;
		/* sets dash length */

		stroke-dashoffset: 0;
		stroke-linecap: round;
		stroke-linejoin: round;
		/* Draw once and done. */
		/* animation: dash 10s linear forwards; */

		/* Keep drawing */
		animation: dash 5s ease-in-out infinite alternate;
		/* animation-delay: 2000ms; */
		/* animation-timing-function: cubic-bezier(0.175, 0.885, 0.32, 1.275); */
	}

	#outliers {
		stroke-dasharray: 1;
		stroke-dashoffset: 0;
		stroke-linecap: round;
		stroke-linejoin: round;
		/* Draw once and done. */
		/* animation: dash 5s linear forwards; */

		/* Keep drawing */
		animation: dash 6s ease-in-out infinite alternate;
	}

	@keyframes dash {
		from {
			stroke-dashoffset: 1;
		}
		to {
			stroke-dashoffset: 0;
		}
	}
</style>
