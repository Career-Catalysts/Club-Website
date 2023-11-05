<script lang="ts">
	import * as Card from '$lib/components/ui/card'
</script>

<Card.Root class="max-w-2xl">
	<Card.Header>
		<Card.Title>Card Title</Card.Title>
		<Card.Description>Card Description</Card.Description>
	</Card.Header>
	<Card.Content>
		<img src="deer.jpg" alt="" />
		<p>Card Content</p>
	</Card.Content>
	<Card.Footer>
		<p>Card Footer</p>
	</Card.Footer>
</Card.Root>
