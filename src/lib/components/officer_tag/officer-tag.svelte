<script lang="ts">
  import * as Avatar from "$lib/components/ui/avatar";

  export let imagePath: string = "officer_pics/Default_pfp.svg";
  export let name: string = "todo";
  export let title: string = "todo";
  export let year: string = "todo";
  export let major: string = "todo";
  export let text_size: number = 2;
</script>

<!-- <div class="w-[45rem] h-[22rem] rounded-md mx-5 flex items-start px-10 py-8 bg-gradient-to-t from-cyan-600 to-blue-700"> -->
<div
  class="rounded-xl w-[rem] px-10
   flex items-start border bg-card text-card-foreground shadow"
>
  <div class="flex flex-col items-center pt-6">
    <Avatar.Root class="flex-shrink-0">
      <Avatar.Image src={imagePath} alt={name} />
      <Avatar.Fallback>CN</Avatar.Fallback>
    </Avatar.Root>
    <h1 class="text-{text_size}xl font-semibold mt-2">{name}</h1>
    <h1 class=" text-sm">{title}</h1>
  </div>

  <div class=" flex-grow text-center p-4">
    <h1 class="p-2">{year}</h1>

    <h1 class="p-2">{major}</h1>
    <h1 class="p-2">fun fact?</h1>
    <h1 class="p-2">contact info</h1>
  </div>
</div>

<style>
</style>
