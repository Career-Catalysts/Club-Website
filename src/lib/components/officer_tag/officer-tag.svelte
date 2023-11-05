<script lang="ts">
  import * as Avatar from "$lib/components/ui/avatar";

  export let imagePath: string = "officer_pics/Default_pfp.svg";
  export let name: string = "todo";
  export let title: string = "todo";
  export let year: string = "todo";
  export let major: string = "todo";
  export let size: number = 5;
</script>

<!-- <div class="w-[45rem] h-[22rem] rounded-md mx-5 flex items-start px-10 py-8 bg-gradient-to-t from-cyan-600 to-blue-700"> -->
<div
  class="rounded-xl w-[{size*9}rem] px-{size *2} 
  py-{size} flex items-start border bg-card text-card-foreground shadow"
>
  <div class="flex flex-col items-center">
    <Avatar.Root class="flex-shrink-0">
      <Avatar.Image src={imagePath} alt={name} />
      <Avatar.Fallback>CN</Avatar.Fallback>
    </Avatar.Root>
    <h1 class="text-{(size * 2) / 5}xl font-semibold mt-2">{name}</h1>
    <h1>{title}</h1>
  </div>

  <div class=" flex-grow justify-center items-center h-full text-center p-4">
    <h1>{year}</h1>
    <h1>{major}</h1>
    <h1>fun fact?</h1>
  </div>
</div>

<style>
</style>
