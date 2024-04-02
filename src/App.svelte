<script>
  import ParNumero from "./components/ParNumero.svelte";
  import Paises from "./components/Paises.svelte";

  const lista =["colombia", "venezuela", "ecuador", "peru", "brasil"]

</script>



<main>
  <div class="">
    <h1 class="title">Identificador de numeros pares e impares</h1>
    <ParNumero/>
  </div>
  <div class="">
    <h1 class="title">Lista de paises</h1>
    {#each lista as pais }
      <div>
        <Paises {pais}/>
      </div>
    {:else}
      no existe elementos
    {/each}  
  </div>  
</main>

<svelte:head>
  <title>Actividad Svelte</title>
</svelte:head>

<style>
  .title{
    color: black;
    font-size: 2em;
    margin-bottom: 50px;
  }
  main{
    display: flex;
    gap: 10rem;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    background-color: #ffffff;
    padding: 2rem;
  }

</style>