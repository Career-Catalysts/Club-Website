<script lang="ts">
	let out_col = 'grey'
	let team_col = 'blue'
</script>

<!-- first page -->
<div
	class="flex items-center justify-center min-w-[40rem] w-[80%] max-w-[77vw]"
>
	<!-- left section: tagline -->
	<aside id='left-section' class="flex bg-[#0d1320]">
	<!-- <aside id='left-section' class="flex"> -->
		<section class="flex flex-col justify-center">
			<h1 class="mb-7 max-w-4xl text-8xl font-medium">
				Turning Interviews Into <u
					class="decoration-purple-500 decoration-5">Opportunities.</u
				>
			</h1>
			<h2 class="max-w-3xl text-6xl font-semibold">
				<mark class="px-1 text-inherit bg-purple-500 rounded-sm"
					>Together</mark
				> We Succeed.
			</h2>
		</section>
	</aside>

	<!-- right section: visual -->
	<aside id='visual' class="w-[40%] min-w-[25rem] pt-16">
		<section>

			<svg viewBox="0 0 500 500">
				<path
					class="outliers"
					pathLength="1"
					stroke="green"
					stroke-width="5"
					fill="none"
					d="M 100 50 l 0 50 l -25 50 l 0 50 l 25 25 l 0 25 l -30 30 l 0 50"
				/>
				<path
					class="team"
					pathLength="1"
					stroke="blue"
					stroke-width="5"
					fill="none"
					d="M 175 50 l 0 50 l 35 50 l 0 150 l -25 50"
				/>
				<path
					class="team"
					pathLength="1"
					stroke="purple"
					stroke-width="5"
					fill="none"
					d="M 250 50 l 0 50 l 0 50 l 0 150 l 0 50"
				/>
				<path
					class="team"
					pathLength="1"
					stroke="orange"
					stroke-width="5"
					fill="none"
					d="M 325 50 l 0 50 l -35 50 l 0 150 l 25 50"
				/>

				<path
					class="outliers"
					pathLength="1"
					stroke="brown"
					stroke-width="5"
					fill="none"
					d="M 400 50 l 0 50 l 25 50 l 0 25 l -50 50 l 0 25 l 50 40 l 0 50 "
				/>

				<path
					d="M143 370c0-11.0457 8.95431-20 20-20h173c11.046 0 20 8.95431 20 20v45c0 11.0457-8.9547 20-20 20h-173c-11.0457 0-20-8.9543-20-20v-200z"
					fill="rgb(168, 85, 247)"
				/>
				<a href="/discover">
					<text class="text-2xl font-semibold" x="190" y="400" fill="white"
						>Learn More</text
					>
				</a>
			</svg>
			<!-- <img src="github.svg" alt="" width="100" height="100" /> -->
		</section>
	</aside>
</div>

<!-- second page; scroll down to see -->
<div class="min-w-[50rem] w-[100vw] max-w-[77vw] px-11">
</div>

<style>
	path {
		stroke-dasharray: 1;

		stroke-dashoffset: 0;
		stroke-linecap: round;
		stroke-linejoin: round;

		animation: dash 5s ease-in-out infinite alternate;
	}

	/* #left-section {
		background: radial-gradient(
			circle at 42% 5%,
			rgba(123, 123, 123, 1) 0%,
			rgba(50, 50, 50, 1) 26%,
			rgba(0, 0, 0, 1) 52%
		);
	} */

	@keyframes dash {
		0% {
			stroke-dashoffset: 1;
		}
		70% {
			stroke-dashoffset: 0;
		}
		100% {
			stroke-dashoffset: 0;
		}
	}

	@media (width < 900px) {
		h1 {
			font-size: 4rem;
		}
		h2 {
			font-size: 3rem;
		}
		#visual {
			min-width: 20rem;
		}
	}
</style>
