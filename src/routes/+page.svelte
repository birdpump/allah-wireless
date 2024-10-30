<script>
    import Carousel from 'svelte-carousel'
    import CarouselItem from "$lib/components/CarouselItem.svelte";
</script>

<style>
    .main-container {
        display: flex;
        flex: 1;
        flex-direction: column;
        height: 100vh;
        /*overflow: hidden;*/
    }

    .carousel {
        flex: 1;
        width: 100%;
        height: 100%;
    }
</style>

<div class="main-container">
    <div class="carousel">
        <Carousel
                autoplay
                autoplayDuration={4500}
                arrows={false}
                swiping={false}
                dots={false}
        >

            <CarouselItem imageUrl="/allah.jpg" text="We are Allah Wireless Communications"/>

            <CarouselItem imageUrl="/allah2.jpeg" text="Delivering coverage to 5M people"/>

            <CarouselItem imageUrl="/microwave.jpg" text="Advanced Terrestrial Microwave services"/>

            <CarouselItem imageUrl="/5g.jpg" text="Featuring high speed 5G technology"/>

            <CarouselItem imageUrl="/tower.jpg" text="Largest towers in the east coast"/>

        </Carousel>
    </div>

</div>