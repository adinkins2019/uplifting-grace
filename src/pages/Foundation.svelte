<script>
    import Page from "../components/Page.svelte"
    import ImageBox from "../components/imageBox.svelte";
    let images = [
        {
            title: "STREAM Education",
            imageUrl: "",
            description: "We believe in providing children with the opportunity to learn 21st century skills and prepare to be leaders of a global economy",
            altText: ""
        },
        {
            title: "Community Development",
            imageUrl: "",
            description: "We believe that everyone should have adequate housing, opportunities for employment, good roads, and methods of transportation.",
            altText: ""
        },
        {
            title: "Health & Nutrition",
            imageUrl: "",
            description: "We believe that people should have nutritious food and access to proper healthcare without paying exorbitant amounts for them.",
            altText: ""
        }
    ]
</script>

<Page>
    <section id="foundation-hist">
        <h2>Our Foundation</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
    </section>
    <section id="foundation-issues">
        <h3>Target Areas</h3>
        <div id="focus-areas">
            {#each images as image}
                <ImageBox 
                  title={image.title}
                  description={image.description} 
                  imageUrl={image.imageUrl} 
                  altText={image.altText} />
            {/each}
        </div>
    </section>
    <section>

    </section>
</Page>

<style>
    section{
        padding: 2%;
    }
    #foundation-issues h3{
        font-weight: 700;
        font-size: 1.25rem;
        text-align: center;
    }
    #focus-areas {
        display: flex;
        justify-content: space-between;
        margin: 0 2%;
    }
</style>