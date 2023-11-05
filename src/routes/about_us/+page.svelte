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
    text_size={2}
  />

  <gap />

  <OfficerTag 
    name="Kenric Tee" 
    title="Vice President" 
    year="1st Year"
    major="Computer Science" 
  />


  <gap />

  <OfficerTag 
    name="Sharvin ..." 
    title="President" 
    year="1st Year" 
  />
  <gap />
  <OfficerTag 
    name="Albert Felix" 
    title="Treasurer" 
    year="1st Year" 
    major="Computer Engineering"
  />
  <gap />
  <OfficerTag
    name="Luis ..."
    title="Public Relations Manager"
    year="1st Year"
    major="Computer Science"
  />
</div>

<style>
  .wrapper {
    width: clamp(50rem, 100%, 68rem);
  }
</style>
