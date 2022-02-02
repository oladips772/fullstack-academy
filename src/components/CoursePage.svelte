<script>
  import Course from "../shared/Course.svelte";
  import { fade, slide, scale, crossfade, fly } from "svelte/transition";

  export let CourseImage;
  export let CourseTitle;
  export let CourseInfo;
  export let CourseStack;
  export let CourseSkills;
  export let CourseReq;
  export let CourseBadge;
</script>

<div class="course-page" transition:fly={{ x: 300, duration: 2000 }}>
  <div class="courses">
    <Course />
    <Course />
    <Course />
    <Course />
    <Course />
    <Course />
    <Course />
    <Course />
  </div>
</div>

<style>
  .courses {
    margin: 120px 40px 50px 90px;
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-gap: 30px;
  }
</style>
