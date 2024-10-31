<script>
    import {onMount} from 'svelte';
    import {scale} from 'svelte/transition';

    export let videoUrl = '';
    export let text = '';

    let visible = false;

    onMount(() => {
        visible = true;
    });
</script>

<style>
    .carousel-element {
        height: calc(100vh - 60px);
        overflow: hidden;
        position: relative;

        display: flex;
        align-items: center;
        justify-content: center;
        overflow: hidden;
    }

    .carousel-text {
        font-weight: bold;
        font-size: 80px;
        text-align: center;
        color: white;
        text-shadow: 5px 5px 10px rgba(0, 0, 0, 0.8);
        position: absolute;
        z-index: 1;
    }

    @media only screen and (max-width: 600px) {
        .carousel-element {
            height: 100vh;
        }

        .carousel-text {
            font-size: 40px;
        }
    }

    video {
        position: absolute;
        top: 50%;
        left: 50%;
        min-width: 100%;
        min-height: 100%;
        width: auto;
        height: auto;
        transform: translate(-50%, -50%);
        z-index: 0;
    }
</style>

<div class="carousel-element">
    <video autoplay loop muted>
        <source src={videoUrl} type="video/mp4"/>
        Your browser does not support the video tag.
    </video>
    {#if visible}
        <div class="carousel-text" transition:scale="{{axis: 'y', delay: 400, duration: 1000}}">{text}</div>
    {/if}
</div>
