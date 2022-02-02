<script>
  export let CourseImage;
  export let CourseInfo;
  export let CourseTitle;
  export let CourseStack;
  export let CourseSkills;
  export let CourseReq;
  export let CourseBadge;
</script>

<div class="course">
  <div class="course-side">
    <img src="/images/course.jpg" alt="" />
    <div class="buttons">
      <button class="front-end">Front End</button>
      <button class="months">3-5 months</button>
    </div>
  </div>
  <div class="course-info">
    <h2>ReactJs / Javascript library</h2>
    <p>
      Master the most popular and most demanding javavscript library out there,
      used to build fast-scalable websites and mobile apps.
    </p>
    <div class="course-skill">
      <h4>Skills Covered</h4>
      <p>
        React-hooks,state-management,props and prop-management,re-usable
        components,conditional-chaining
      </p>
    </div>
    <div class="course-req">
      <h4>Pre-requisites</h4>
      <p>HTML , CSS , JavaScript , Es6</p>
    </div>
  </div>
</div>
   
<style>
  .course {
    width: 550px;
    height: 100%;
    padding: 30px 10px;
    display: flex;
    align-items: center;
    border-radius: 6px;
    background: white;
    box-shadow: 0px 0px 2px 4px rgba(241, 240, 240, 0.993);
    -webkit-box-shadow: 0px 2px 5px 3px rgba(231, 228, 228, 0.966);
    -moz-box-shadow: 0px 0px 3px 4px rgba(236, 234, 234, 0.719);
  }
  .course-side {
    display: flex;
    flex-direction: column;
    align-items: center;
    border-right: 1px solid grey;
    padding-right: 5px;
    height: 100%;
  }
  .course-side img {
    height: 100px;
    width: 100px;
    border-radius: 6px;
    object-fit: cover;
    margin-bottom: 20px;
  }
  .buttons {
    display: flex;
    flex-direction: column;
    margin: 10px;
    font-size: 17px;
  }
  .buttons button {
    height: 30px;
    width: 100px;
    border-radius: 5px;
    align-items: center;
    text-align: center;
  }
  .course-info {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    width: 100%;
    height: 100%;
    margin-top: -16px;
    margin-left: 10px;
  }
  .course-info p {
    font-size: 16px;
  }
  .course-info h2 {
    margin-bottom: 6px;
    /* font-weight: normal; */
    width: 100%;
    color: gray;
  }
  .course-info h4 {
    margin-bottom: 5px;
    width: 100%;
    color: rgb(29, 190, 42);
  }
  .course-skill {
    width: 100%;
    margin-top: 8px;
    margin-bottom: 5px;
  }
  .course-req {
    width: 100%;
  }
  .front-end {
    color: rgb(29, 190, 42);
    background-color: rgb(255, 255, 255);
    height: 40px;
    border-color: rgb(29, 190, 42);
    border: 2px solid;
    font-size: 14px;
    text-align: center;
  }
  .months {
    color: rgb(255, 255, 255);
    background-color: rgb(29, 190, 42);
    height: 40px;
    border: none;
    margin-top: 12px;
    font-size: 14px;
    text-align: center;
  }
</style>
