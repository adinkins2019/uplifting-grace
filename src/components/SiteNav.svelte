<script>
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

<nav>
    <ul>
        {#each navUrls as navUrl}
        <li><a href={navUrl.url}>{navUrl.name}</a></li>
        {/each}
    </ul>
 
</nav>