<script>
  import * as d3 from "d3"

  export let numbers = []

</script>
 
<div class="car-container">
  {#each numbers as n}
  <div>
    <div class="row-wrapper">
      <div class="row-car" style="width: {n}px;  background-color: green;"></div>
      <img class="car" src="./images/autocompleto.png" alt="">
    </div>
    <p class="number">{n}%</p>
  </div>
  {/each}
</div>

<style>
  .car-container {
    display: flex;
    margin-top: -150px;
    justify-content: center;
  }
  .row-wrapper {
    position: relative;
    width: 200px;
    height: 120px;
  }
  .row-car {
    position: absolute;
    bottom: 20px;
    left: 28px;
    height: 60px;
  }
  .car {
    position: absolute;
    z-index: 1;
    bottom: 0;
  }
  .number {
    position: absolute;
    text-align: center;
    font-family: 'Roboto', sans-serif;
  }
</style>