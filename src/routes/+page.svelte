<script>
    import Carousel from 'svelte-carousel'
    import CarouselItem from "$lib/components/CarouselItem.svelte";
    import VideoItem from "$lib/components/VideoItem.svelte";
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
                arrows={false}
                autoplay
                autoplayDuration={4500}
                dots={false}
                swiping={false}
        >
            <VideoItem videoUrl="https://d1bz9hu881c3qi.cloudfront.net/sites/video1.mp4" text="We Are Allah Wireless Communications"/>

            <CarouselItem imageUrl="/connect.jpg" text="Pioneering the Future of Communication"/>

            <CarouselItem imageUrl="/microwave.jpg" text="Advanced Terrestrial Microwave Services"/>

            <CarouselItem imageUrl="/data.jpg" text="24/7 Field Proven Reliability"/>

            <CarouselItem imageUrl="/5g.jpg" text="High-Speed 5G Technology"/>

            <CarouselItem imageUrl="/tower.jpg" text="Tallest Towers on the West Coast"/>

            <VideoItem videoUrl="https://d1bz9hu881c3qi.cloudfront.net/sites/radio.mp4" text="Bridging Distances Farther Than Ever Before"/>

            <CarouselItem imageUrl="/networks.jpg" text="Smart Networks Today for Tomorrows Solutions"/>

            <CarouselItem imageUrl="/allah2.jpeg" text="Delivering Impeccable Coverage to Over 5M Customers"/>
        </Carousel>
    </div>
</div>