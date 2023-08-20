<script>
    export let img
</script>

<main>
    <p class="item">• Sobre mí</p>
    <h1 class="titulo">Me llamo Laureano Neyén Chaves</h1>
    <p class="desc">Actualmente tengo 22 años, resido en la ciudad de Arrecifes, provincia Buenos Aires, Argentina. Me encuentro estudiando Ingeniería en Sistemas de la Información en la Universidad Tecnológica Nacional de Rosario.</p>
    <br>
    <p class="desc">Siempre estoy intentando mejorar mis cualidades en como el trabajo en equipo, la comunicación y flexibilidad. Siento que fortalecer esas cualidades es muy importante para lograr el objetivo principal de mi carrera como profesional.</p>
    <br>
    <p class="desc">Busco crear sistemas informaticos útiles y usables para facilitarles la vida a las personas. Por ultimo, me encanta cocinar y ver las partidas competitivas de KOI, un equipo de Esports. </p>

    <img src="{img}" alt="Chaves Laureano Neyén Foto"/>
</main>

<style>
    main{
      width: 25%;
      margin: auto;
      display: flex;
      flex-direction: column;
      max-width: 600px;
      background-color: white;
      padding: 1.25rem;
      border-radius: 0.75rem;
      box-shadow: 0px 10px 10px rgba(0, 0, 0, 0.13);
      margin-top: 2rem; 
    }

    .item{
        margin-top: 1rem;
        font-size: 0.75rem;
        margin-bottom: 1.5rem;
    }
    .titulo{
        margin-bottom: 1rem;
        font-weight: 800;
      font-size: 1.5rem;
    }

    .desc{
        
        color:#666D80;
        font-weight: 500;
        line-height: 1.8;
    }
</style>