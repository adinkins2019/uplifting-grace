<script>
    import {Route} from 'svelte-routing'
    import AboutUs from '../pages/AboutUs.svelte'
    import ContactUs from '../pages/ContactUs.svelte'
    import Foundation from '../pages/Foundation.svelte'
    import Home from '../pages/Home.svelte'
    import Products from '../pages/Products.svelte'
</script>

<div>
    <Route path="/" component={Home}/>
    <Route path="products" component={Products}/>
    <Route path="about-us" component={AboutUs}/>
    <Route path="/social-responsibility" component={Foundation}/>
    <Route path="/contact-us" component={ContactUs}/>
</div>