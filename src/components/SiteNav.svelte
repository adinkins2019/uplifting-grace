<script>
    import {Link} from 'svelte-routing'
    export let pageClass;
    let navUrls = [
        {
            url: '/',
            name: 'Home'
        },
        {
            url: '/products',
            name: 'Products'
        },
        {
            url: '/about-us',
            name: 'About Us'
        },
        {
            url: '/social-responsibility',
            name: 'Our Foundation'
        },
        {
            url: '/contact-us',
            name: 'Contact Us'
        }
    ]
</script>

<nav class={pageClass ? 'pageHeader': ''}>
    <ul>
        {#each navUrls as navUrl}
        <li><Link to={navUrl.url}>{navUrl.name}</Link></li>
        {/each}
    </ul>
 </nav>
 <style>
     .pageHeader {
         background: #E4BE9E;
         width: 75%;
     }
     li {
         list-style-type: none;
         margin-bottom: 2px;
         font-size: 0.75rem;
     }
     .pageHeader ul {
         display: flex;

     }
     .pageHeader ul li {
         padding: 2%;
         font-size: 1.15rem;
     }

     
 </style>