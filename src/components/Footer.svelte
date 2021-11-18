<footer>
  <div class="foot1">
    <div class="logo">
      <img
        src="https://www.jobboardfinder.com/upload/7480cf6f7ec084752d8e78ca4f021bd37c1b30eb/logo_jobboard.png"
        alt=""
      />
      <h2>Full Stack Developer Academy</h2>
    </div>
    <div class="text">
      <p>
        Our experts work with you to design a tailored transformation journey.
        Solve your acute workforce challenges to deliver next-level business
        results.
      </p>
    </div>
    <div class="icons">
      <i class="fab fa-instagram" /> 
      <i class="fab fa-facebook-f" />
      <i class="fab fa-twitter" />
      <i class="fab fa-linkedin-in" />
    </div>
  </div>
  <div class="foot2">
    <h4>Get in Touch</h4>
    <div class="contact-icons">
      <div class="phone">
        <i class="fas fa-phone-volume" />
        <p>+234 595 5554 22</p>
      </div>
      <div class="mail">
        <i class="far fa-envelope" />
        <p>FullStack@gmail.com</p>
      </div>
      <div class="mail">
        <i class="fas fa-map-marker-alt" />
        <p>British America</p>
      </div>
    </div>
  </div>
  <div class="foot3">
    <h4>Our Services</h4>
    <div class="services">
      <p>Machine learning</p>
      <p>Tech Bootcamp/coding cohort</p>
      <p>Mobile App Developement</p>
      <p>Web Services / Developement</p>
      <p>Women Technology Programs</p>
    </div>
  </div>
</footer>

<style>
  footer {
    background: black;
    width: 100%;
    color: white;
    display: flex;
    align-items: center;
    justify-content: space-around;
  }
  .foot1 {
    padding: 15px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    width: 350px;
    margin-bottom: 10px;
  }
  .foot2{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
    width: 250px;
    height: 220px;
  }
  .foot2 .contact-icons {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin-top:0;
  }
  .foot2 h4{
    margin-bottom:-80px;
    margin-left:-80px;
  }
  .foot3{
    margin-top:-30px;
  }
  .services{
    display:flex;
    flex-direction: column;
    align-items:center;
    justify-content: space-between;
    width:100%;
  }
  .services p{
    margin:5px 0;
    width:100%;
    cursor: pointer;
  }
  .foot3 h4{
    margin-bottom:10px;
  }
  .foot1 p {
    margin-bottom: 23px;
    line-height: 25px;
    margin-top: 5px;
  }
  .logo {
    display: flex;
    align-items: center;
    color: white;
    margin-left: -40px;
  }
  .logo img {
    height: 50px;
  }
  .logo h2 {
    font-size: 17px;
  }
  .icons i {
    color: white;
    font-size: 20px !important;
    cursor: pointer;
    transition: all 0.3s ease
  }
  .icons i:hover{
    color:rgb(53, 211, 53);
  }
  .foot1 .icons {
    display: flex;
    justify-content: space-around;
    align-items: center;
    width: 100%;
    margin-left: -60px;
  }
  .foot2 .contact-icons {
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
  .phone,
  .mail {
    margin-bottom: 10px;
    display: flex;
    align-items: center;
    width:100%;
    cursor: pointer;
    transition: all 0.3s ease;
  }
  .phone:hover{
    color:rgb(53, 211, 53);
  }
   .mail:hover{
    color:rgb(53, 211, 53);
  }
  .phone i {
    margin-right: 14px;
  }
  .mail i {
    margin-right: 14px;
  }
</style>
