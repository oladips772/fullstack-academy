<script>
  import { fade, slide, scale, crossfade, fly } from "svelte/transition";

  const profile = [
    {
      id: 1,
      Name: "Elon Musk",
      Designation: "full stack developer",
      Description:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
      profileImg:
        "https://cdn.vox-cdn.com/thumbor/wDvmcj9eEin57A1Nww0yBM1jASc=/1400x1400/filters:format(jpeg)/cdn.vox-cdn.com/uploads/chorus_asset/file/22386618/1229901940.jpg",
    },
    {
      id: 2,
      Name: "Elon Musk",
      Designation: "full stack developer",
      Description:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
      profileImg:
        "https://imageio.forbes.com/specials-images/imageserve/5ec595d45f39760007b05c07/0x0.jpg?format=jpg&crop=1491,1490,x989,y74,safe&fit=crop",
    },
    {
      id: 3,
      Name: "Elon Musk",
      Designation: "full stack developer",
      Description:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
      profileImg:
        "https://cdn.vox-cdn.com/thumbor/wDvmcj9eEin57A1Nww0yBM1jASc=/1400x1400/filters:format(jpeg)/cdn.vox-cdn.com/uploads/chorus_asset/file/22386618/1229901940.jpg",
    },
    {
      id: 4,
      Name: "Elon Musk",
      Designation: "full stack developer",
      Description:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
      profileImg:
        "https://cdn.vox-cdn.com/thumbor/wDvmcj9eEin57A1Nww0yBM1jASc=/1400x1400/filters:format(jpeg)/cdn.vox-cdn.com/uploads/chorus_asset/file/22386618/1229901940.jpg",
    },
  ];

  let index = 0;
  const next = () => {
    index = (index + 1) % profile.length;
  };
  const prev = () => {
    index = (index - 1) % profile.length;
  };
</script>

<main>
  <div class="outerDiv">
    {#each [profile[index]] as person (index)}
      <div
        class="profileDiv"
        id="profileDiv"
        transition:fly={{ x: 200, duration: 1000 }}
      >
        <div class="control-div">
          <img
            src="https://www.pngarts.com/files/2/Left-Arrow-PNG-Free-Download.png"
            alt=""
            class=" icon left-icon"
            id="left"
            on:click={prev}
          />
          <img
            src="https://www.pngarts.com/files/2/Left-Arrow-PNG-Free-Download.png"
            alt=""
            class=" icon right-icon"
            id="right"
            on:click={next}
          />
          <img src={person.profileImg} alt="ll" class="profileImg" />
        </div>
        <div class="infoDiv">
          <span>Name:</span>
          <h4>{person.Name}</h4>
          <span>Designation:</span>
          <h4>{person.Designation}</h4>
          <span>Description:</span>
          <h4>{person.Description}</h4>
        </div>
      </div>
    {/each}
  </div>
</main>

<style>
  main {
    height: 100vh;
    margin: 90px 80px;
  }
  .outerDiv {
    display: flex;
    max-width: 700px;
    margin: 0 auto;
    width: 100%;
    overflow: hidden;
  }
  .profileDiv {
    display: flex;
    justify-content: space-between;
    align-items: center;
    /* border: 1px solid #000; */
  }
  .control-div {
    position: relative;
  }
  .profileImg {
    height: 400px;
    width: 300px;
    background-position: center;
    border-radius: 5px;
  }
  .infoDiv {
    width: 400px;
    height: 100%;
    margin-left: 10px;
    margin: 20px 10px;
  }
  h4 {
    width: 100%;
    margin-bottom: 20px;
  }
  .icon {
    height: 25px;
    object-fit: contain;
    position: absolute;
    bottom: 20px;
    right: 20px;
    cursor: pointer;
  }
  .right-icon {
    bottom: 60px;
    transform: rotate(180deg);
  }
  span {
    color: purple;
    padding: 5px;
    font-weight: bold;
    margin: 10px 0px;
  }
</style>
