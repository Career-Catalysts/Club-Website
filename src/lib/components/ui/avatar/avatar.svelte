<script lang="ts">
  import { Avatar as AvatarPrimitive } from "bits-ui";
  import { cn } from "$lib/utils";

  type $$Props = AvatarPrimitive.Props;

  let className: $$Props["class"] = undefined;
  export let delayMs: $$Props["delayMs"] = undefined;
  //TODO figure out a way to make this scalable
  export let height: string = "h-[6rem]"; // Default height
  export let width: string = "w-[6rem]"; // Default width
  export { className as class };
</script>

<AvatarPrimitive.Root
  {delayMs}
  class={cn(
    "relative flex shrink-0 overflow-hidden rounded-full",
    height, // Include the 'height' prop
    width, // Include the 'width' prop
    className
  )}
  {...$$restProps}
>
  <slot />
</AvatarPrimitive.Root>
