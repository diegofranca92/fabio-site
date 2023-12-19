<script>
  import Counter from './Counter.svelte'
  import welcome from '$lib/images/svelte-welcome.webp'
  import fotoPerfil from '$lib/images/fabio.png'
</script>

<svelte:head>
  <title>Home</title>
  <meta name="description" content="Fabio Site" />
</svelte:head>

<section>
  <img class="foto-perfil" src={fotoPerfil} alt="" />
  <div>
    <h1>Prof. Fabio</h1>

    <h2>Sou professor de Fisica</h2>
  </div>
</section>

<style>
  .foto-perfil {
    width: 300px;
    height: 300px;
    border-radius: 50%;
  }
  section {
    display: flex;
		align-items: center;
		justify-content: center;
		gap: 40px;
  }

  h1 {
    width: 100%;
  }

  .welcome {
    display: block;
    position: relative;
    width: 100%;
    height: 0;
    padding: 0 0 calc(100% * 495 / 2048) 0;
  }

  .welcome img {
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    display: block;
  }
</style>
