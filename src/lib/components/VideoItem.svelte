<script>
    export let videoUrl = ''; // Change from imageUrl to videoUrl
    export let text = '';
</script>

<style>
    .carousel-element {
        height: calc(100vh - 60px); /* Adjust as needed */
        overflow: hidden;
        position: relative; /* Make this relative for absolute positioning of video */

        display: flex;
        align-items: center;
        justify-content: center;
        overflow: hidden; /* Ensure overflow is hidden for the video */
    }

    .carousel-text {
        font-weight: bold;
        font-size: 80px;
        text-align: center;
        color: white;
        text-shadow: 5px 5px 10px rgba(0, 0, 0, 0.8);
        position: absolute; /* Position text over the video */
        z-index: 1; /* Ensure text is above the video */
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
        position: absolute; /* Position video absolutely to fill the element */
        top: 50%;
        left: 50%;
        min-width: 100%; /* Ensure the video fills the width */
        min-height: 100%; /* Ensure the video fills the height */
        width: auto; /* Allow width to auto adjust */
        height: auto; /* Allow height to auto adjust */
        transform: translate(-50%, -50%); /* Center the video */
        z-index: 0; /* Ensure video is behind the text */
    }
</style>

<div class="carousel-element">
    <video autoplay muted loop>
        <source src={videoUrl} type="video/mp4" />
        Your browser does not support the video tag.
    </video>
    <div class="carousel-text">{text}</div>
</div>
