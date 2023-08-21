<script>
export let item, tit, desc, href, img, alt, src

</script>


<main>

    <p class="item">{item}</p>
    <p class="titulo">{tit}</p>
    <p class="desc">{desc}</p>
    <a class="ref" href="{href}" target="_blank">Visitar</a>
    <img src="{img}" alt="{alt}"/>
    
    {#if src=="vid"}
    video
    {/if}

    

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
        margin-bottom: 1rem;
    }

    .ref {
        margin: 1rem 0;
        background-color: #6B4EFF;
        padding: 0.5rem 1rem;
        border-radius: 0.75rem;
        width: 3rem;
        color: white;
        cursor: pointer;
    }

    @media (max-width: 450px) {

main{
width: 90%;

}
}
</style>