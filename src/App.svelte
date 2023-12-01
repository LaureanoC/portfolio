<script>

import {Router, Route, Link} from 'svelte-routing'
import Home from './views/Home.svelte'
import About from './views/About.svelte'
import Education from './views/Education.svelte'
import Contacto from './views/Contacto.svelte'
import Dolar from './views/Dolar.svelte'
import Tryhard from './views/Tryhard.svelte'
import Foodtruck from './views/Foodtruck.svelte'
import Academia from './views/Academia.svelte'

export let clase = 1; 

function cambiarClase(e) {
    if(e.target.classList[1] == 'fa-house'){
        clase = 1
    }
    if(e.target.classList[1] == 'fa-user'){
        clase = 2
    }
    if(e.target.classList[1] == 'fa-graduation-cap'){
        clase = 3
    }
    if(e.target.classList[1] == 'fa-address-book'){
        clase = 4
    }

}

</script>


<header>
	
		<Router>
			<div class="container">
				<Link to="/"><i class="fa-solid fa-house {clase == 1 ? "actual" : ""}" on:click={cambiarClase}></i></Link>
				<Link to="/about"><i class="fa-solid fa-user {clase == 2 ? "actual" : ""}" on:click={cambiarClase} ></i></Link>
				<Link to="/education"><i class="fa-solid fa-graduation-cap {clase == 3 ? "actual" : ""}" on:click={cambiarClase} ></i></Link>
				<Link to="/contact"><i class="fa-solid fa-address-book {clase == 4 ? "actual" : ""}" on:click={cambiarClase} ></i></Link>
                <div class="brands">
                    
                    <a href="https://instagram.com/laureano.chaves" target="_blank"><i class="fa-brands fa-instagram"></i></a>
                    <a href="https://github.com/LaureanoC" target="_blank"><i class="fa-brands fa-github-alt"></i></a>
                    <a href="https://www.linkedin.com/in/laureano-neyén-chaves/" target="_blank"><i class="fa-brands fa-linkedin-in"></i></a>



                </div>
			</div>
			<Route path="/"><Home/></Route>
			<Route path="/about"><About img="yo2.jpg"/></Route>
			<Route path="/education"><Education/></Route>
            <Route path="/contact"><Contacto/></Route>
            <Route path="/dolarblueactual"><Dolar/></Route>
            <Route path="/foodtruck"><Foodtruck/></Route>
            <Route path="/tryhardzone"><Tryhard/></Route>
            <Route path="/academia"><Academia/></Route>
		</Router>
	
</header>



<style>


header {
    margin-top: 2rem;
    
    
}
.container{
    width: 25%;
    margin: auto;
    display: flex;
    max-width: 600px;
    gap: 1.5rem;
    background-color: white;
    padding: 1.25rem;
    border-radius: 0.75rem;
    box-shadow: 0px 5px 5px rgba(0, 0, 0, 0.13);   
}


.fa-house{
    margin-left: 1rem;
}

i{
    color: rgb(107, 78, 255, .37)
    
}

i:hover{
    color: rgb(107, 78, 255, 100);
    transition: 1s;
}

.actual{
    color: rgb(107, 78, 255);
}

.brands{
    margin-left: auto;
    display: flex;
    gap: 1rem;
}


@media (max-width: 450px) {

    .container{
        width: 90%;
        
    }
}
    


</style>