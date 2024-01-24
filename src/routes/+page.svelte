<!-- <script lang='ts'>

</script>

 -->
<script>
	import { DeviceMockup } from 'flowbite-svelte'

	import { Button } from '$lib/components/ui/button'
</script>

<DeviceMockup device="ios">
	<div class="p-20">
		<h1>Welcome to SvelteKit</h1>
		<p>
			Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation
		</p>
	</div>

	<Button>Button</Button>
</DeviceMockup>

<DeviceMockup device="laptop">
	<div class="p-20">
		<h1>Welcome to SvelteKit</h1>
		<p>
			Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation
		</p>
	</div>
</DeviceMockup>
