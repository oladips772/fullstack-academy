<script>
  import { Link } from "svelte-routing";
</script>

<main>
  <!-- svelte-ignore a11y-label-has-associated-control -->
  <!-- svelte-ignore a11y-label-has-associated-control -->
  <form>
    <div class="input-zz">
      <img src="/images/main-logo.png" alt="" />
      <input type="text" id="Name" placeholder="Name" />
      <input type="text" id="Email" placeholder="Email" />
      <input type="password" id="Password" placeholder="Password" />
      <button>Sign Up</button> <button>Log In</button>
      <div>
        <button class="google">Sign In With Google</button>
      </div>
    </div>
  </form>
</main>

<style>
  main {
    background-image: url(/images/login-background.jpg);
    background-repeat: no-repeat;
    object-fit: contain;
    background-size: cover;
    top: 0;
    right: 0;
    left: 0;
    bottom: 0;
    height: 100vh;
    width: 100%;
  }
  form {
    top: 50%;
    left: 50%;
    position: absolute;
    transform: translate(-50%, -50%);
    background: white;
    max-width: 600px;
    width: 80%;
    height: 70%;
    margin: 0 auto;
    /* padding: 15px 10px 10px 10px; */
    border-radius: 10px;
  }
  form .input-zz {
    display: block;
    margin: 0 auto;
    text-align: center;
  }
  button {
    color: rgb(31, 197, 31);
    background-color: white;
    border-color: rgb(31, 197, 31);
    height: 40px;
    width: 120px;
    border-radius: 10px;
    border: 1px solid;
    font-size: 20px;
  }
  .google {
    color: white;
    background-color: rgb(31, 197, 31);
    width: 250px;
    margin: 20px;
  }
  .input-zz input {
    display: block;
    margin: 0 auto;
    height: 35px;
    width: 80%;
    margin-bottom: 14px;
    font-size: 18px;
    outline: none;
    border: none;
    border-bottom: 1px solid black;
    /* padding: 10px; */
  }
  .input-zz img {
    height: 70px;
  }
</style>
