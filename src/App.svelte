<script>
	
	import Header from "./components/Header.svelte";
	import {Router} from 'svelte-routing'
	import Routes from './routes/Routes.svelte'

	export let url = ""
</script>

<Router url="{url}">
	<Header />
	<Routes />
</Router>
