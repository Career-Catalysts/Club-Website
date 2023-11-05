<script lang="ts">
	import { Avatar as AvatarPrimitive } from "bits-ui";
	import { cn } from "$lib/utils";
  
	type $$Props = AvatarPrimitive.Props;
  
	let className: $$Props["class"] = undefined;
	export let delayMs: $$Props["delayMs"] = undefined;
	export let height: string = "h-60"; // Default height
	export let width: string = "h-60";   // Default width
	export { className as class };
  </script>
  
  <AvatarPrimitive.Root
	{delayMs}
	
	class={cn(
	  "relative flex shrink-0 overflow-hidden rounded-full",
	  height, // Include the 'height' prop
	  width,  // Include the 'width' prop
	  className
	)}
	{...$$restProps}
  >
	<slot />
  </AvatarPrimitive.Root>