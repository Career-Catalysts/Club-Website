<script lang="ts">
  import * as Avatar from "$lib/components/ui/avatar";
</script>

<div class="w-[45rem] h-[22rem] rounded-md mx-5 flex items-start px-10 py-8 bg-gradient-to-t from-cyan-600 to-blue-700">
    <div class="flex flex-col items-center">
      <Avatar.Root class="flex-shrink-0">
        <Avatar.Image src="officer_pics/Default_pfp.svg" alt="officerpic" />
        <Avatar.Fallback>CN</Avatar.Fallback>
      </Avatar.Root>
      <h1 class="text-2xl  font-semibold mt-2">Name</h1>
    </div>
  </div>
  
  
<style>
</style>
