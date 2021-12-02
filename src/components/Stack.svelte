<div class="stack">
  <div class="stack-header">
    <h2>Choose your stack!</h2>
  </div>
  <div class="stack-images">
    <img src="/images/html.png" alt="" title="HTML5" />
    <img src="/images/css3.png" alt="css3.png" title="CSS3" />
    <img src="/images/javascript.png" alt="javascript.png" title="JavaScript" />
    <img src="/images/NODE.jpg" alt="node.png" title="NodeJs" />
    <img src="/images/PHP.svg" alt="PHP.svg" title="PHP" />
    <img src="/images/react.png" alt="react.png" title="ReactJs" />
  </div>
</div>

<style>
  .stack {
    margin-top: 80px;
    margin-bottom: 120px;
  }
  .stack-images {
    margin-top: 35px;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
  .stack-images img {
    height: 75px;
    width: 75px;
    border-radius: 50%;
    padding: 5px;
    object-fit: contain;
    /* box-shadow: rgb(53, 211, 53) 1px 1px 1px 1px; */
    cursor: pointer;
    transition-delay: 0.2s;
    transition: 1s linear;
  }
  .stack-images img:hover {
    transform: rotate(362deg);
    transition-delay: 0.2s;
  }
</style>
