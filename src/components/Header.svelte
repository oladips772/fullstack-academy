<script>
/**@format*/
let closeBtn = document.querySelector(".fa-times");
let navBtn = document.getElementsByClassName(".fa-bars");
const Navz = document.getElementsByClassName(".links-tab");
let active = document.querySelector(".active");

let showModal = true;
import {
    Link
} from "svelte-routing";

const showNav = () => {
    Navz.active();
    console.log(Navz);
};
</script>

<!-- svelte-ignore a11y-invalid-attribute -->
<div class="header">
    <div class="logo">
        <img
            src="https://www.jobboardfinder.com/upload/7480cf6f7ec084752d8e78ca4f021bd37c1b30eb/logo_jobboard.png"
            alt=""
            />
        <h3>Fullstack</h3>
    </div>
    <i class="fas fa-times" />
    <div class="links-tab">
        <Link to="/">Home</Link>
        <Link to="#"
        >Courses
        <i class="fa fa-sort-down" />
        </Link>
        <Link to="#"
        >Alumni
        <i class="fa fa-sort-down" />
        </Link>
        <Link to="#"
        >Contact Us
        <i class="fa fa-sort-down" />
        </Link>
        <Link to="#">Help</Link>
    </div>
    <div class="enroll">
        <button class="sign-btn">Sign In</button>
        <!-- svelte-ignore a11y-missing-attribute -->
        <Link to="/Login">
        <button class="enroll-btn">Enroll</button>
        </Link>
    </div>
    <i class="fas fa-bars" on:click={showNav} />
</div>

<style>
.header {
    display: flex;
    align-items: center;
    justify-content: space-around;
    height: 60px;
    transition: all 0.3s ease;
    box-shadow: rgba(0, 0, 0, 0.35) 0px 1px 7px;
    background: white;
    width: 100%;
    top: 0;
    z-index: 9;
    position: fixed;
    margin-bottom: 30px;
}

.logo {
    display: flex;
    align-items: center;
    transition: all 0.3s ease-in;
    margin-right: 170px;
}

.logo h3 {
    display: none;
    transition: all 0.9s ease;
    cursor: pointer;
    transform: translateX(-20%);
    font-size: 0;
}

.logo:hover img {
    display: none;
    transition: all 0.9s ease;
}

.logo:hover h3 {
    display: block;
    transform: translateX(-20%);
    transition: all 0.9s ease;
    font-size: 18px;
}

.header img {
    height: 55px;
    object-fit: contain;
}

.links-tab {
    border-right: 2px solid gray;
    height: 40%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    text-align: center;
    margin-right: -110px;
}

.links-tab a {
    align-items: center;
    display: flex;
    text-decoration: none;
    justify-content: space-between;
    margin-right: 50px;
    color: black;
    font-size: 19px;
    transition: all 0.3s ease;
    padding: 4px;
    border-radius: 3px;
}

.links-tab a:hover {
    /* border-top: 2px solid rgb(53, 211, 53);
      border-right: 2px solid black; */
    color: rgb(53, 211, 53);
}

.links-tab a i {
    margin-left: 10px;
    align-items: center;
    margin-top: -8px;
    color: black;
}

.enroll {
    display: flex;
}

.enroll button {
    border: none;
    outline: none;
    background: none;
    font-size: 18px;
    cursor: pointer;
    color: black;
    transition: all 0.3s ease;
}

button.sign-btn:hover {
    color: rgb(53, 211, 53);
}

.enroll .enroll-btn {
    background: rgb(53, 211, 53);
    padding: 7px 15px 7px 15px;
    border-radius: 3px;
    color: white;
    text-transform: uppercase;
    font-size: 14px;
    margin-left: 35px;
}

.fa-bars {
    display: none;
}

.fa-times {
    display: none;
}

/* media queries */
@media (max-width: 1060px) {
    .fa-bars {
        display: block;
        font-size: 27px !important;
        color: rgb(53, 211, 53);
    }

    .links-tab {
        display: none;
        height: 100%;
        min-height: 800px;
        background: rgb(53, 211, 53);
        color: white;
        position: absolute;
        width: 200px;
        top: 1px;
        border: none;
        right: 110px;
    }

    .links-tab.active {
        display: block;
        height: 100%;
        min-height: 800px;
        background: rgb(53, 211, 53);
        color: white;
        position: absolute;
        width: 200px;
        top: 1px;
        border: none;
        right: 110px;
    }

    .links-tab a {
        height: 60px;
        color: white;
        width: 100%;
        margin-top: 20px;
        font-size: 25px;
    }

    .links-tab a:hover {
        color: white;
    }

    .links-tab a i {
        margin-right: 15px;
    }

    .enroll {
        display: none;
    }

    .fa-times {
        display: block;
        font-size: 30px !important;
        position: absolute;
        top: 10px;
        right: 20px;
        color: white;
        z-index: 9;
    }
}
</style>
