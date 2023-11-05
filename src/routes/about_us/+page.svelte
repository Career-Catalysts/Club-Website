<script>
  import * as Avatar from "$lib/components/ui/avatar";
  import OfficerTag from "$lib/components/officer_tag/officer-tag.svelte";
</script>

<!-- <div class="max-w-6xl"> -->
<div class="grid grid-cols-3 gap-4">
  <OfficerTag
    name="Surendra Jammishetti"
    title="Director of Research"
    year="1st Year"
    major="Computer Engineering"
    text_size={1}
  />

  <gap />

  <OfficerTag />

  <gap />

  <OfficerTag />
  <gap />
  <OfficerTag />
  <gap />
  <OfficerTag />
</div>

<style>
  .wrapper {
    width: clamp(50rem, 100%, 68rem);
  }
</style>
