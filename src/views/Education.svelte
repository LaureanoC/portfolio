<script>
import Item from './components/Item.svelte'
</script>

<main>
    <p class="item">• Formación académica</p>
    <h1 class="titulo">Mis estudios</h1>
    <p class="desc">He realizado dos cursos sobre desarrollo web y estoy estudiando ingeniería en sistemas, me encuentro entre tercer y cuarto año de la rama principal.</p>
    <br>

    <div class="container__item">
        <p class="item__titulo">• Educación</p>
        <a href="/dolarblueactual"><Item subtitulo = "Ingeniería en Sistemas de la Información" desc="2019 - Actualidad (18/35)" img="utn.png"  chevron="true"/></a>
        <a href="/foodtruck"><Item subtitulo = "Oracle Next Education" desc="2022 - Oracle y Alura Latam" img="oracle.png" chevron="true"/></a>
        <a href="/tryhardzone"><Item subtitulo = "Formación Fullstack Python" desc="2021 - Codo a codo 4.0" img="codo.png" chevron="true"/></a>
      </div>
  
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

    .container__item{
      background-color: #F6F8FA;
      margin: 1rem 0;
      border-radius: 0.75rem;
      padding-bottom: 1rem;
    }
  
    .item__titulo{
      margin-left: 1rem;
      font-size: 0.75rem;
      margin-top: 1rem;
    }

</style>