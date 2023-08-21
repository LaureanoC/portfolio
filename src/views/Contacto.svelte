<script>



</script>

<main>
    <p class="item">• Contacto</p>
    <p class="titulo">Envíame un correo</p>
    <p class="desc">¿Quieres contactarme? Complete el siguiente formulario y me pondré en contacto lo antes posible</p>
    <form action="https://formspree.io/f/xrgwqejr" method="POST"
>
    <input  type="text" placeholder="Nombre" name="nombre" required/>
    <input  type="email" placeholder="Email" name="email" required/>
    <textarea name="mensaje" placeholder="Mensaje" required></textarea>
  <button type="submit">Enviar</button>
</form>

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

    form {
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
    }

    input{
        background-color: #F1F4F8;
        padding: 1rem;
        border-radius: 0.75rem;
        margin-bottom: 1rem;
        font-family: 'Inter', sans-serif;
    }

    textarea{
        background-color: #F1F4F8;
        flex-basis: 100%;
        resize: none;
        font-family: 'Inter', sans-serif;
        padding: 1rem;
    }

    button{
        margin-top: 1rem;
        background-color: #6B4EFF;
        font-family: 'Inter', sans-serif;
        padding: 0.5rem 1rem;
        border-radius: 0.75rem;
        color: white;
        cursor: pointer;
    }

    @media (max-width: 450px) {

main{
width: 90%;
}

input{
    flex-basis: 100%;
}
}
</style>