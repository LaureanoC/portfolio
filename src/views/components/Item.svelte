<script>
export let subtitulo
export let desc
export let img
export let chevron
</script>

<div class="container">
    <img src="{img}" alt="{subtitulo}"/>
    <div class="container__desc">
        <p class="subtitulo">{subtitulo}</p>
        <p class="desc">{desc}</p>
    </div>

    {#if chevron=="true"}
    <i class="fa-solid fa-chevron-right"></i>
    {/if}
    
</div>

<style>

.container {
    display: flex;
    background-color: white;
    align-items: center;
    border-radius: 0.75rem;
    padding: 0.75rem;
    margin: 1rem 2rem;
    gap: 1rem;
    box-shadow: 0px 5px 5px rgba(0, 0, 0, 0.13);
}

.container__desc{
    display: flex;
    flex-direction: column;
    
}

.subtitulo{
    font-weight: 500;
    font-size: 0.75rem;
    margin: 0;
}

.desc{
    font-size: 0.625rem;
    margin: 0;
}

img{
    width: 50px;
    border-radius: 5rem;
    box-shadow: 0px 3px 3px rgba(0, 0, 0, 0.13); 
}

.fa-chevron-right{
    margin-left: auto;
    margin-right: 1rem;
    color: #797F90;
    font-size: 0.625rem;
}
</style>