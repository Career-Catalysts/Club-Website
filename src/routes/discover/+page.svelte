<script>
	import * as Accordion from '$lib/components/ui/accordion'
	import * as Tabs from '$lib/components/ui/tabs'
	import * as Card from '$lib/components/ui/card'
	import '../../app.postcss'
</script>

<div class="flex flex-col gap-9 m-auto wrapper h-fit">
	<div
		class="bg-gradient-to-t from-purple-500 to-blue-600 rounded-md text-left py-3 px-12"
	>
		<h2 class="">TLDR</h2>
		<p>
			We believe that our efforts to share resources and knowledge can not
			only help the community out there striving towards a common goal, we
			will also appreciate all the moral support of like-minded individuals
			out there.

			<!-- We believe our
		resource sharing and knowledge exchange can assist like-minded individuals
		and communities striving for common goals, and we value their moral
		support. -->
		</p>
	</div>

		<Tabs.Root value="Goal">
			<Tabs.List
				class="grid w-full h-auto grid-cols-3 bg-inherit text-white border-purple-500 border-[5px]"
			>
				<Tabs.Trigger value="Goal" class="text-3xl font-normal"
					>Goal</Tabs.Trigger
				>
				<Tabs.Trigger value="Values" class="text-2xl font-normal"
					>Values</Tabs.Trigger
				>
				<Tabs.Trigger value="Mission" class="text-2xl font-normal"
					>Mission</Tabs.Trigger
				>
			</Tabs.List>
			<Tabs.Content value="Goal" class="text-xl">
				<Card.Root>
					<Card.Content class="p-5 h-[27rem]">
						<div class="py-3 px-7 text-left">
							<p
								class="bg h-auto text-center rounded-md text-white mb-5 leading-10"
							>
								<!-- Create an environment where peers are encouraging
							and helping one another improve in 3 main areas.  -->

								Cultivate a collaborative environment for like-minded
								individuals to excel in three key areas.
							</p>

							<div class="flex justify-between space-x-5">
								<h3 class="bg">
									Communication: Can you get your point across in an
									articulate manner?
									<img src="deer.jpg" alt="" />
								</h3>
								<h3 class="bg">
									Confidence: Do you do well under pressure? Have you
									ever blanked out?
								</h3>
								<h3 class="bg">
									Community: Would you rather tackle challenges alone
									or with your peers?
								</h3>
							</div>
						</div>
					</Card.Content>
				</Card.Root>
			</Tabs.Content>
			<Tabs.Content value="Values">
				<Card.Root>
					<Card.Content class="p-5 h-[27rem]">
						<div class="py-3 px-7 text-left">
							<p
								class="bg h-auto text-center rounded-md text-white mb-3 leading-10"
							>
								Transparency & Honesty, Support & Growth
							</p>
						</div>
					</Card.Content>
				</Card.Root>
			</Tabs.Content>
			<Tabs.Content value="Mission">
				<Card.Root>
					<Card.Content class="p-5 h-[27rem]">
						<div class="py-3 px-7 text-left">
							<p
								class="bg h-auto text-center rounded-md text-white mb-3 leading-10"
							>
								To learn and grow with like-minded community members in
								pursuit of internship opportunities.
							</p>
						</div>
					</Card.Content>
				</Card.Root>
			</Tabs.Content>
		</Tabs.Root>

	<div class="flex gap-7 justify-between wrapper">
		<div
			class="rounded-md p-5 w-1/3 bg-gradient-to-t from-purple-500 to-blue-600"
		>
			<h2>Who we are.</h2>
			<p>
				Believe it or not, we are just as lost as you are in the search for
				an internship. We are a group of Freshman looking to bolster our
				career and secure a stronghold for our future. So, what better place
				to start this journey than college?
			</p>
		</div>
		<div
			class="rounded-md p-5 w-1/3 bg-gradient-to-t from-purple-500 to-blue-600"
		>
			<h2>Who we are not.</h2>
			<p>
				We are not a bunch of Freshman trying to teach about the
				interviewing process. Rather, we are here to learn with you. That
				said, we try our best to prepare our meetings such that you learn AT
				LEAST 1 new valuable thing each time.
			</p>
		</div>
		<div
			class="rounded-md p-5 w-1/3 bg-gradient-to-t from-purple-500 to-blue-600"
		>
			<h2>Why we came to be.</h2>
			<p>
				In this era where AI is booming, tech and finance internships are
				only getting more competitive by the year. The ultimate question
				that brought us together is: How do we improve our chances & stand
				out? Does that resonate with you?
			</p>
		</div>
	</div>

	<!-- FAQ: - What is this club about? - Is this club for you?
	
Resources: Compilation of links (guides, blogs, videos) to valuable resources -->
	<div class="text-6xl p-5 pb-52">
		<h2 class="text-left underline">FAQ</h2>
		<Accordion.Root>
			<Accordion.Item value="item-1">
				<Accordion.Trigger class="text-3xl font-light"
					>What is this club about?</Accordion.Trigger
				>
				<Accordion.Content class="text-xl">
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Beatae,
					aut.
				</Accordion.Content>
			</Accordion.Item>
			<Accordion.Item value="item-2">
				<Accordion.Trigger class="text-3xl font-light"
					>Is this club for you?</Accordion.Trigger
				>
				<Accordion.Content class="text-xl">
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio,
					maiores!
				</Accordion.Content>
			</Accordion.Item>
		</Accordion.Root>
	</div>
</div>

<style>
	.wrapper {
		width: clamp(50rem, 100%, 68rem);
	}

	h1 {
		font-size: 3rem;
	}

	h2 {
		font-size: 2rem;
	}

	h3 {
		width: 33%;
		padding: 1rem 2rem;
		border-radius: calc(var(--radius) - 2px);
		color: white;
		text-align: center;
	}

	p {
		font-size: 1.5rem;
		padding: 0.5rem 1.5rem;
	}

	.bg {
		background: linear-gradient(
			180deg,
			rgba(13, 19, 32, 1) 0%,
			rgba(8, 12, 21, 1) 100%
		);
	}

</style>
