<script>
    export let imageUrl = '';
    export let text = '';

</script>

<style>
    .carousel-element {
        /*width: 100%;*/
        height: calc(100vh - 60px);
        overflow: hidden;
        background-size: cover;
        background-position: center;
        background-repeat: no-repeat;

        display: flex;
        align-items: center;
        justify-content: center;
    }

    .carousel-text {
        font-weight: bold;
        font-size: 80px;
        text-align: center;
        color: white;
        text-shadow: 5px 5px 10px rgba(0, 0, 0, 0.8);
    }

    img {
        width: 100%;
        height: 100%;
        object-fit: cover;
    }
</style>

<div class="carousel-element" style="background-image: url({imageUrl});">
    <!--    <img src={imageUrl} alt=""/>-->
    <div class="carousel-text">{text}</div>
</div>