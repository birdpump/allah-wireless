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
                autoplayDuration={3500}
                arrows={false}
                swiping={false}
                dots={false}
        >

            <CarouselItem imageUrl="/allah.jpg" text="We are Allah Wireless Communications"/>

            <CarouselItem imageUrl="/microwave.jpg" text="Advanced Terrestrial Microwave services"/>

            <CarouselItem imageUrl="/data.jpg" text="24/7 Proven reliability"/>

            <CarouselItem imageUrl="/5g.jpg" text="High speed 5G technology"/>

            <CarouselItem imageUrl="/tower.jpg" text="Tallest towers in the west coast"/>

            <CarouselItem imageUrl="/allah2.jpeg" text="Delivering impeccable coverage to over 5M customers"/>

        </Carousel>
    </div>

</div>