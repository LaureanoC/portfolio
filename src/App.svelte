<script>

import {Router, Route, Link} from 'svelte-routing'
import Home from './views/Home.svelte'
import About from './views/About.svelte'


</script>


<header>
	
		<Router>
			<div class="container">
				<Link to="/"><i class="fa-solid fa-house"></i></Link>
				<Link to="/about"><i class="fa-solid fa-user"></i></Link>
				<Link to="/education"><i class="fa-solid fa-graduation-cap"></i></Link>
				<Link to="/contact"><i class="fa-solid fa-address-book"></i></Link>
			</div>
			<Route path="/"><Home/></Route>
			<Route path="/about"><About img="yo2.jpg"/></Route>
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


</style>