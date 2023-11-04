<script lang="ts">
  import Button from "$lib/components/ui/button/button.svelte";
  let out_col = "grey";
  let team_col = "blue";
  //   const pauseAnimation = () => {
  //     const team = document.getElementsByClassName(
  //       "team"
  //     ) as HTMLCollectionOf<HTMLDivElement>;
  //     for (const t of team) {
  //       if (t.style) {
  //         t.style.animationPlayState = "paused";
  //       } else {
  //         console.log("team is null");
  //       }
  //     }
  //   };

  //   const resumeAnimation = () => {
  //     const team = document.getElementsByClassName(
  //       "team"
  //     ) as HTMLCollectionOf<HTMLDivElement>;
  //     for (const t of team) {
  //       if (t.style) {
  //         t.style.animationPlayState = "running";
  //       } else {
  //         console.log("wtf happened");
  //       }
  //     }
  //   };
</script>

<!-- <div class="max-w-6xl"> -->
<div
  class="flex items-center justify-center min-w-[50rem] w-[90%] max-w-[70vw] h-full"
>
  <aside class="flex">
    <section class="flex flex-col justify-center">
      <h1 class="mb-11 max-w-2xl text-7xl font-medium">
        Turning Interviews Into Opportunities.
      </h1>
      <h2 class="max-w-2xl text-5xl font-semibold">Together We Succeed.</h2>
    </section>
  </aside>

  <aside class="w-[40%]">
    <section>
      <!-- <Button on:click={pauseAnimation}>Pause</Button>
        <Button on:click={resumeAnimation}>Resume</Button> -->
      <svg viewBox="0 0 500 500">
        <path
          class="outliers"
          pathLength="1"
          stroke={out_col}
          stroke-width="3"
          fill="none"
          d="M 100 50 l 0 50 l -25 50 l 0 50 l 25 25 l 0 25 l -30 30 l 0 50"
        />
        <path
          class="team"
          pathLength="1"
          stroke={team_col}
          stroke-width="3"
          fill="none"
          d="M 175 50 l 0 50 l 35 50 l 0 150 l -25 50"
        />
        <path
          class="team"
          pathLength="1"
          stroke={team_col}
          stroke-width="3"
          fill="none"
          d="M 250 50 l 0 50 l 0 50 l 0 150 l 0 50"
        />
        <path
          class="team"
          pathLength="1"
          stroke={team_col}
          stroke-width="3"
          fill="none"
          d="M 325 50 l 0 50 l -35 50 l 0 150 l 25 50"
        />

        <path
          class="outliers"
          pathLength="1"
          stroke={out_col}
          stroke-width="3"
          fill="none"
          d="M 400 50 l 0 50 l 25 50 l 0 25 l -50 50 l 0 25 l 50 40 l 0 50 "
        />

        <path
          d="M143 370c0-11.0457 8.95431-20 20-20h173c11.046 0 20 8.95431 20 20v45c0 11.0457-8.9547 20-20 20h-173c-11.0457 0-20-8.9543-20-20v-200z"
          fill="#90EE90"
        />
      </svg>
      <!-- <img src="github.svg" alt="" width="100" height="100" /> -->
    </section>
  </aside>
</div>

<style>
  path {
    stroke-dasharray: 1;

    stroke-dashoffset: 0;
    stroke-linecap: round;
    stroke-linejoin: round;

    animation: dash 5s ease-in-out infinite alternate;

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

</style>
