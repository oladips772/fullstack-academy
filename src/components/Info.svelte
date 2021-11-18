<script>
</script>

<div class="Info">
  <article>
    <div class="info-text">
      <h2>Radical talent <br /> transformation is here.</h2>
      <p>
        Changing lives, businesses, and nations through <br /> talent transformation
        in digital technologies.
      </p>
    </div>
    <div class="images">
      <img
        class="firstImg"
        src="https://www.uneca.org/sites/default/files/styles/tumbnail_436_x_221/public/storyimages/shutterstock_1854693433.jpg?itok=-EOUtSZj"
        alt=""
      />
      <img
        class="secondImg"
        src="https://www.motocms.com/blog/wp-content/uploads/2019/11/how-to-become-a-web-developer.jpg"
        alt=""
      />
      <img
        class="thirdImg"
        src="https://images.unsplash.com/photo-1571171637578-41bc2dd41cd2?ixid=MnwxMjA3fDB8MHxzZWFyY2h8N3x8d2ViJTIwZGV2ZWxvcG1lbnR8ZW58MHx8MHx8&ixlib=rb-1.2.1&w=1000&q=80"
        alt=""
      />
    </div>
  </article>
  <div class="enroll">
    <div class="front-end">
      <button class="test-btn">Enroll</button>
      <h4>Front End</h4>
    </div>
    <div class="back-end">
      <button>Enroll</button>
      <h4>Back End</h4>
    </div>
  </div>
</div>

<style>
  .Info {
    margin-top: 100px;
    height: 100%;
    width: 100%;
    background-image: url(/images/9.png);
    background-repeat: no repeat;
    background-size: cover;
    margin-bottom: 40px;
    padding-bottom: 20px;
  }
  img {
    height: 150px;
    width: 150px;
    object-fit: cover;
    border-radius: 7px;
    transition: all 0.3s ease;
  }
  img:hover {
    transform: translateY(-10px);
    border-radius: 7px;
  }
  img:hover.secondImg {
    border-top-right-radius: 7px;
    border-bottom-left-radius: 33px;
    transition: all 0.3s ease;
  }
  img:hover.firstImg {
    border-top-left-radius: 7px;
    border-bottom-right-radius: 33px;
    transition: all 0.3s ease;
  }
  img:hover.thirdImg {
    border-bottom-right-radius: 7px;
    border-top-left-radius: 33px;
    transition: all 0.3s ease;
  }
  .images .firstImg {
    border-top-left-radius: 33px;
    position: absolute;
    right: 100px;
  }
  .images .secondImg {
    border-top-right-radius: 33px;
    position: absolute;
    bottom: 230px;
    right: 300px;
  }
  .images .thirdImg {
    border-bottom-right-radius: 33px;
    position: absolute;
    right: 100px;
    bottom: 60px;
  }

  article {
    display: flex;
    justify-content: space-between;
  }
  h2 {
    font-size: 60px;
  }
  .info-text p {
    font-size: 30px;
    margin-top: 25px;
  }

  /* enroll button div styling */
  .enroll {
    display: flex;
    margin-top: 60px;
    padding: 10px;
  }
  .front-end {
    display: flex;
    align-items: center;
    justify-content: space-around;
    flex-direction: column;
    height: 110px;
    width: 230px;
    margin-right: 30px;
    border-radius: 8px;
    box-shadow: rgba(143, 99, 99, 0.35) 2px 2px 2px 1px;
    border-left: 6px solid rgb(53, 211, 53);
    transition: all 0.3s ease;
    background: white;
  }
  .back-end {
    display: flex;
    align-items: center;
    justify-content: space-around;
    flex-direction: column;
    height: 110px;
    width: 230px;
    border-radius: 8px;
    box-shadow: rgba(143, 99, 99, 0.35) 2px 2px 2px 1px;
    border-left: 6px solid crimson;
    transition: all 0.3s ease;
    background: white;
  }
  .back-end:hover {
    border-left: none;
    border-bottom: 6px solid crimson;
    box-shadow: rgba(143, 99, 99, 0.35) 2px 1px 1px;
    transition: all 0.3s ease;
  }
  .front-end:hover {
    border-left: none;
    border-bottom: 6px solid rgb(53, 211, 53);
    box-shadow: rgba(143, 99, 99, 0.35) 2px 1px 1px;
    transition: all 0.3s ease;
  }
  .enroll button {
    border-radius: 4px;
    font-size: 18px;
    height: 38px;
    width: 120px;
    cursor: pointer;
    outline: none;
    border: none;
    background: rgb(53, 211, 53);
    color: white;
    font-weight: 600;
    transition: all 0.3s ease;
  }

  .enroll h4 {
    font-size: 20px;
  }
</style>
