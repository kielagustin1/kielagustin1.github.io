<!-- src/App.svelte -->
<script>
	import { Router, Route } from 'svelte-routing';
	import Nav from './components/Nav.svelte';
	import Home from './routes/Home.svelte';
	import Portfolio from './routes/Portfolio.svelte';
	import About from './routes/About.svelte';
	import Contact from './routes/Contact.svelte';
  </script>
  
  <Router>
	<Nav />
	<main>
	  <Route path="/" component={Home} />
	  <Route path="/portfolio" component={Portfolio} />
	  <Route path="/about" component={About} />
	  <Route path="/contact" component={Contact} />
	</main>
  </Router>
  