<script>
    import Page from "../components/Page.svelte"
    import ContactForm from "../components/ContactForm.svelte";
</script>

<Page>
    <section id="content-description">
        <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>
    </section>
    <section>
        <div id="contact-form">
            <ContactForm />
        </div>
    </section>

        
    <section></section>
</Page>

<style>
    #content-description{
        padding: 3%;
        font-size: 1.15rem;
    }
    #contact-form {
        width: 70%;
        margin: 0 auto;
        font-size: 1.15rem; 
    }
</style>