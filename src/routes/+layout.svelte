<script>
    import TopNav from "$lib/components/TopNav.svelte";
</script>

<style>
    /* todo fix weird layout shift on google when keyboard deployed */
    .layout-main {
        font-family: "Montserrat", sans-serif;
        background-color: var(--background);
        color: var(--text);
        display: flex;
        flex-direction: column;
        height: 100%;
        position: absolute;
        width: 100vw;
    }
</style>

<svelte:head>
    <title>Allah Wireless</title>

    <meta name="description" content="Allah Wireless Communications offers impeccable coverage, high-speed 5G, and advanced communications services to millions.">
    <meta name="keywords" content="Allah Wireless, allah wireless, allah wireless communications, wireless communication, 5G, microwave services, telecom, coverage, reliable internet">
</svelte:head>

<div class="layout-main">
    <TopNav/>
    <slot/>
</div>