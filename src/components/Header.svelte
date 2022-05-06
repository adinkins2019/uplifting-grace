<script>
    import SiteNav from "./SiteNav.svelte"
    function handleClick(){

    }
</script>

<header class="pageheader">
    <div class="logo">
        <h1>Uplifting Grace</h1>
    </div>
    <div id="nav-links">
      <SiteNav pageClass="page"/>
      <button type="button" on:click={handleClick}>Get Started</button>
    </div>
</header>
<style>
    @import url('https://fonts.googleapis.com/css2?family=Cinzel:wght@400;600;700&display=swap');
    .logo{
        width: 100%;
    }
    .logo h1{
        font-family: 'Cinzel', serif, sans-serif;
        font-weight: 700;
        font-size: 3rem;
        text-transform: uppercase;
        background-image: url("../assets/images/Uplifting.png");
        background-repeat: no-repeat;
        text-align: center;
    }
    

    .pageheader {
        display: flex;
        flex-direction: column;
        justify-content: center;
    }
    #nav-links{
        display: flex;
        justify-content: space-between;
        background: #E4BE9E;
    }

   #nav-links button {
       margin-top: 10px;
       margin-right: 2%;
       height: 35%;
       padding: 2%;
       border-radius: 5px;
       background: #71697A;
       color: #E4BE9E;
       border: 2px solid #71697A;
   }  

   #nav-links button:hover {
       transition-duration: 0.5s;
       transform: scale(1.1);
       background: #E4BE9E;
       color: #71697A;
   }
</style>