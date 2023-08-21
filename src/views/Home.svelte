<script>
    import {Link} from 'svelte-routing'
import Item from "./components/Item.svelte";
  </script>
  
  <main>
    <p class="dot">• Estudiante de Ingeniería en Sistemas</p>
  
    <div class="container__top">
      <div>
        <p class="titulo">Soy Laureano Chaves</p>
        <p class="titulo__desc">Futuro Ingeniero en Sistemas de la Información.</p>
      </div>
      <img src="yo.png" alt="Foto de Laureano Neyén Chaves"/>
      
    </div>
  
    <div class="container__item">
      <p class="item__titulo">• Proyectos</p>
      <Link to="/dolarblueactual"><Item subtitulo = "Dólar blue hoy" desc="Realizada con Svelte." img="dolar.png"  chevron="true"/></Link>
      <Link to="/foodtruck"><Item subtitulo = "Foodtruck" desc="Carrito de comidas realizado con Java." img="carrito.png" chevron="true"/></Link>
      <Link to="/tryhardzone"><Item subtitulo = "TryhardZone" desc="E-commerce realizado con Javascript." img="ecommerce.png" chevron="true"/></Link>
    </div>
  
    <div class="container__item">
      <p class="item__titulo">• Hard skills</p>
      <Item subtitulo = "MySQL" desc="Creación de base de datos y consultas complejas." img="mysql.png" chevron="false"/>
      <Item subtitulo = "Java" desc="JDBC y JSP sin Frameworks." img="java.png" chevron="false"/>
      <Item subtitulo = "Svelte" desc="Lo esencial para desarrollar aplicaciones web." img="svelte.png" chevron="false"/>
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
    
    a{
      text-decoration: none;
      color: inherit;
    }
  
    .dot {
      margin-top: 1rem;
      font-size: 0.75rem;
      
    }
  
    .titulo{
      font-weight: 800;
      font-size: 1.5rem;
    }
  
    .titulo__desc{
      color: #666D80;
      font-size: 1.125rem;
      font-weight: 500;
      margin-top: 0.5rem;
    }
  
    .container__top{
      display: flex;
      align-items: center;
      justify-content: space-between;
  
    }
  
    img {
      width: 125px;
      height: 125px;
      border-radius: 5rem;
      box-shadow: 0px 10px 10px rgba(0, 0, 0, 0.13);
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

@media (max-width: 450px) {

        main{
        width: 90%;
    
}
}
  </style>