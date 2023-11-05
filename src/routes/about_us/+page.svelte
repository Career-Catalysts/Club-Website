<script>
  import * as Avatar from "$lib/components/ui/avatar";
  import OfficerTag from "$lib/components/officer_tag/officer-tag.svelte";
</script>

<!-- <div class="max-w-6xl"> -->
<div class="wrapper grid grid-cols-3 gap-4">
  <OfficerTag
    name="Surendra J."
    title="Director of Research"
    year="1st Year"
    major="Computer Engineering"
    text_size={2}
  />

  <svg viewBox="0 0 500 175">
    <path
      class="outliers"
      pathLength="1"
      stroke="green"
      stroke-width="5"
      fill="none"
      d="M 10 20 l 50 50 l 100 0 l 25 25 l 100 0 l 125 0 l 25 -25 l 50 0"
    />
  </svg>

  <OfficerTag
    name="Kenric T."
    title="Vice President"
    year="1st Year"
    major="Computer Science"
  />

  <svg viewBox="0 0 500 175">
    <path
      class="outliers"
      pathLength="1"
      stroke="green"
      stroke-width="5"
      fill="none"
      d="M 10 20 l 50 50 l 100 0 l 25 25 l 100 0 l 125 0 l 25 -25 l 50 0"
    />
  </svg>

  <OfficerTag name="Sharvin S." title="President" year="1st Year" />
  <svg viewBox="0 0 500 175">
    <path
      class="outliers"
      pathLength="1"
      stroke="green"
      stroke-width="5"
      fill="none"
      d="M 10 20 l 50 50 l 100 0 l 25 25 l 100 0 l 125 0 l 25 -25 l 50 0"
    />
  </svg>
  <OfficerTag
    name="Albert F."
    title="Treasurer"
    year="1st Year"
    major="Computer Engineering"
  />
  <svg viewBox="0 0 500 175">
    <path
      class="outliers"
      pathLength="1"
      stroke="green"
      stroke-width="5"
      fill="none"
      d="M 10 20 l 50 50 l 100 0 l 25 25 l 100 0 l 125 0 l 25 -25 l 50 0"
    />
  </svg>
  <OfficerTag
    name="Luis C."
    title="Public Relations Manager"
    year="1st Year"
    major="Computer Science"
    text_size={2}
  />
</div>

<style>
  path {
    stroke-dasharray: 1;

    stroke-dashoffset: 0;
    stroke-linecap: round;
    stroke-linejoin: round;

    animation: dash 5s ease-in-out infinite;
  }

  @keyframes dash {
    0% {
      stroke-dashoffset: 1;
    }
    70% {
      stroke-dashoffset: 0;
    }
    100% {
      stroke-dashoffset: 0;
    }
  }

  @media (width < 900px) {
    h1 {
      font-size: 3.5rem;
    }
    h2 {
      font-size: 2.7rem;
    }
    #visual {
      min-width: 20rem;
    }
  }
  .wrapper {
		width: clamp(40rem, 100%, 80rem);
	}
</style>
