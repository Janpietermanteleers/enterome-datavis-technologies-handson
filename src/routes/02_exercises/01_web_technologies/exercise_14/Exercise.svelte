<script>
  let current = "";
 
</script>


<style>
  pl{
    background-color: red;
    font-size: large;
  }
</style>



<!-- We will cover buttons later on! -->
<button class="{(current == 'messi') ? 'pl' :" btn btn-secondary"}" on:click={() => (current = "messi")}>
  Messi
</button>

<button class="btn btn-secondary" on:click={() => (current = "ronaldo")}>
  Ronaldo
</button>

<button class="btn btn-secondary" on:click={() => (current = "neymar")}>
  Neymar
</button>
