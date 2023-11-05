<script>
	import * as Avatar from '$lib/components/ui/avatar';
	import OfficerTag from '$lib/components/officer_tag/officer-tag.svelte';

</script>

<!-- <div class="max-w-6xl"> -->
<div class="wrapper flex grid-cols-3">
	
	<div class="col-span-1"><OfficerTag></OfficerTag></div>
	<div class="col-span-1"></div>
	<div class="col-span-1"><OfficerTag></OfficerTag></div>
	<div class="col-span-1"><OfficerTag></OfficerTag></div>
	


	

</div>

<style>
	.wrapper {
		width: clamp(50rem, 100%, 68rem);
	}
</style>
