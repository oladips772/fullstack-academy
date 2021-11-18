<script>
  function checkThis(choice) {
    document.getElementById("env-text1").classList.toggle("active");
    choice.target.classList.toggle("active");
  }
  function checkThis2(choice) {
    document.getElementById("env-text2").classList.toggle("active");
    choice.target.classList.toggle("active");
  }
  function checkThis3(choice) {
    document.getElementById("env-text3").classList.toggle("active");
    choice.target.classList.toggle("active");
  }
</script>

<!-- GET now -->
<div class="tech">
  <div class="tech-diff">
    <h2>Tech services</h2>
    <div class="tech-about">
      <h3>Full Stack Developer Academy offers different tech services ...</h3>
      <p>
        Our experts work with you to design a tailored transformation journey. <br
        />
        Solve your acute workforce challenges to deliver next-level business results.
      </p>
    </div>
    <div class="tech-accordion">
      <div class="enviroment-accordion">
        <h3>
          1. Enviroment <i class="fas fa-chevron-down" on:click={checkThis} />
        </h3>
        <div id="env-text1">
          Assess talent gaps to accurately benchmark and prioritize innovation
          projects. Align organizational goals and define workforce
          transformation strategy, with competencies curated to the individual
          level.
        </div>
      </div>
      <div class="enviroment-accordion">
        <h3>
          2. Coaching <i class="fas fa-chevron-down" on:click={checkThis2} />
        </h3>
        <div id="env-text2">
          Use our proven playbook to achieve targeted results that increase
          retention and productivity. Consistently deliver quantifiable outcomes
          that matter to ROI and business growth, while gaining productivity and
          a competitive advantage in the market.
        </div>
      </div>
      <div class="env3">
        <h3 class="env3">
          3. Results <i class="fas fa-chevron-down" on:click={checkThis3} />
        </h3>
        <div id="env-text3" class="env3">
          Use our proven playbook to achieve targeted results that increase
          retention and productivity. Consistently deliver quantifiable outcomes
          that matter to ROI and business growth, while gaining productivity and
          a competitive advantage in the market.
        </div>
      </div>
    </div>
  </div>
  <div class="tech-side-image">
    <img src="/images/222.svg" alt="" class="techImg1" />
    <img src="/images/33333.png" alt="" class="techImg2" />
    <img src="/images/444444.png" alt="" class="techImg3" />
    <img src="/images/2747251.png" alt="" class="techImg4" />
  </div>
</div>

<style>
  .tech {
    margin-bottom: 125px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-top: 80px;
  }
  h2 {
    font-size: 40px;
    margin-bottom: 50px;
    margin-top: 70px;
    border-right: 6px solid rgb(53, 211, 53);
  }
  .tech-diff {
    margin-top: 30px;
  }
  .tech-diff p {
    margin-top: 10px;
    line-height: 24px;
  }
  .tech-accordion {
    margin-top: 20px;
    width: 550px;
  }
  .enviroment-accordion {
    line-height: 26px;
    border-bottom: 2px solid rgb(53, 211, 53);
    margin-bottom: 10px;
    padding-bottom: 10px;
    overflow: hidden;
  }
  .enviroment-accordion h3 {
    cursor: pointer;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .env3 h3 {
    cursor: pointer;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .env3 {
    border-bottom: none;
  }
  .tech-side-image {
    height: 80px;
    position: absolute;
    right: 10px;
    top: 800px;
  }
  .tech-side-image img {
    height: 70px;
    transition: all 0.9s ease-in-out;
  }
  .tech-side-image .techImg1 {
    right: 420px;
    top: 30px;
    position: absolute;
    transition: all 0.9s ease-in-out;
    transition-delay: 0.3s;
  }
  .tech-side-image .techImg2 {
    bottom: -180px;
    right: 250px;
    position: absolute;
    transition: all 0.9s ease-in-out;
    transition-delay: 0.3s;
  }
  .tech-side-image .techImg3 {
    top: 30px;
    right: 50px;
    position: absolute;
    transition: all 0.9s ease-in-out;
    transition-delay: 0.3s;
  }
  .tech-side-image .techImg4 {
    right: 260px;
    top: -140px;
    position: absolute;
    transition: all 0.9s ease-in-out;
    transition-delay: 0.3s;
  }
  .tech-side-image:hover .techImg1 {
    transform: translateX(370px);
  }
  .tech-side-image:hover .techImg3 {
    transform: translateX(-370px);
  }
  .tech-side-image:hover .techImg2 {
    transform: translateY(-330px);
  }
  .tech-side-image:hover .techImg4 {
    transform: translateY(330px);
  }
  .fa-chevron-down {
    transition: all 0.3s ease;
    transition-delay: 0.1s;
  }
</style>
