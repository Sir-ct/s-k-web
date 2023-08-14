<script>
  import { Route, Link, Router, navigate} from 'svelte-routing'
  import Home from './routes/Home.svelte';
  import About from './routes/About.svelte';
    import Blog from './routes/Blog.svelte';
    import Login from './routes/Login.svelte';

    let loggedIn = true
    if(loggedIn){
      navigate('/')
    }else{
      navigate('/login')
    }
    let location = window.location.pathname
    console.log(location)
</script>

<main>
  <Router>
    <Route path='/' component={Home} />
    <Route path='/inventory' component={Home} />
    <Route path='/sales' component={Home} />
    <Route path='/purchases' component ={Home} />
    <Route path='/login' component={Login} />
    <Route path='' component={About} />
  </Router>
</main>
