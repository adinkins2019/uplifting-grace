<script>
    export let description;
    export let imageUrl;
    export let altText;
    export let title;
</script>
<div class="image-container">
    <img src={imageUrl} alt={altText}>
    <div class="imgbox-desc">
        <h4>{title}</h4>
        <p>{description}</p>
    </div>
</div>
<style>
    .image-container{
        border: 2px solid black;
        border-radius: 5%;
        width: 30%;
        height: 75%;
        box-shadow: 5px 10px 5px black;
    }
    .imgbox-desc {
        font-size: 0.95rem;
        padding: 2%;

    }

    .imgbox-desc h4 {
        font-size: 1rem;
        text-align: center;
    }
    .imgbox-desc p {
        padding: 2%;
    }
</style>