<script>
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
        "https://cdn.vox-cdn.com/thumbor/wDvmcj9eEin57A1Nww0yBM1jASc=/1400x1400/filters:format(jpeg)/cdn.vox-cdn.com/uploads/chorus_asset/file/22386618/1229901940.jpg",
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
</script>

<main>
  <div class="outerDiv">
    {#each profile as person}
      <div class="profileDiv">
        <div class="control-div">
          <img src="https://www.pngarts.com/files/2/Left-Arrow-PNG-Free-Download.png" alt="" class=" icon left-icon"/>
          <img src="https://www.pngarts.com/files/2/Left-Arrow-PNG-Free-Download.png" alt="" class=" icon right-icon"/>
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
    /* overflow: hidden; */
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
    width: 100%;
    /* border: 1px solid #000; */
  }
  .control-div{
    position:relative;
  }
  .profileImg {
    height: 400px;
    width: 300px;
    /* object-fit: cover; */
    background-position: center;
    border-radius: 5px;
  }
  .infoDiv {
    width: 400px;
    height: 100%;
    margin-left: 10px;
  }
  h4 {
    width: 100%;
  }
  .icon{
    height:25px;
    object-fit:contain;
    position: absolute;
    bottom: 20px;
    right:20px;
    cursor:pointer;
  }
  .right-icon{
    bottom:60px;
    transform:rotate(180deg);
  }
  span {
    color: purple;
    padding: 5px;
    font-weight: bold;
    margin: 10px 0px;
  }
</style>
