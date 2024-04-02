<script>
  import * as d3 from "d3"
  import CarRows from "./lib/CarRows.svelte"

  let numbers = [5, 18, 29, 75, 100]
</script>

<main>
  <h1 class="headline">Porcentaje de combustible disponible</h1>
  <div class="rectangulo"></div>
  <!-- Canal: altura. Tipo: col con divs -->
  <CarRows numbers={numbers} />
  
</main>

<style>
  .headline {
    text-align: center;
    text-decoration: underline;
    background-color: rgb(99, 99, 99);
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
  }
  .rectangulo{
    width: 2000%;
    height: 150px;
    background-color: rgb(99, 99, 99);
    margin: 0%;
  }
</style>
