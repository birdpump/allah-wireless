<script>

</script>

<style>
    .logo-cont a {
        display: inherit;
    }

    a:link {
        text-decoration: none;
    }

    a:visited {
        text-decoration: none;
    }

    a:hover {
        text-decoration: none;
    }

    a:active {
        text-decoration: none;
    }

    .icon-stack {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        gap: 4px;
        cursor: pointer;
    }

    /* .icon-stack:hover{
        background-color: #101014;
        border-radius: 6px;
    } */

    .stack-text {
        /* font-family: Mo; */
        font-size: 14px;
        color: var(--text);
    }

    .material-symbols-outlined {
        font-variation-settings: "FILL" 0, "wght" 400, "GRAD" 0, "opsz" 24;
        color: var(--text);
        user-select: none;
        cursor: pointer;
        width: 24px;

    }

    .icon-cont {
        margin-right: 20px;
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;
        gap: 35px;
    }

    .logo-cont {
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;
        gap: 8px;
    }

    .top-navigation-container {
        width: 100vw;
        display: flex;
        justify-content: space-between;
        flex-direction: row;
        height: 60px;
    }

    .nav-padding {
        width: 100%;
        padding-right: 12px;
        padding-left: 12px;
    }

    .top-navigation {
        display: flex;
        align-items: center;
        height: 100%;
        width: 100%;
        margin-right: auto;
        margin-left: auto;
        justify-content: space-between;
    }

    .navigation-links {
        display: flex;
        gap: 12px;
        font-weight: 500;
    }

    .nav-link {
        color: var(--text);
        font-size: 16px;
        border-radius: .5rem;
        align-self: center;
        padding: 16px;
        transition: all .2s;

    }

    .nav-link:hover {
        background-color: rgba(0, 0, 0, 0.2);
    }

    .logo {
        height: 20px;
        /*width: 60px;*/
        cursor: pointer;
    }

    .top-text {
        font-size: 18px;
        font-weight: bold;
        color: var(--text);
    }

    @media only screen and (max-width: 1000px) {
        .top-text {
            display: none;
        }

    }

    @media only screen and (max-width: 600px) {
        .top-navigation-container {
            display: none;
        }

    }
</style>

<div class="top-navigation-container">
    <div class="nav-padding">
        <div class="top-navigation">
            <div class="logo-cont">
                <div class="top-text">Allah Wireless</div>
                <a href="/"><img alt="cv logo" class="logo" loading="eager" rel="preload" src="/wifi.svg"/></a>
            </div>

            <div class="navigation-links">
                <a href="/" class="nav-link">Home</a>

                <a href="/orgs" class="nav-link">About</a>

                <a href="/help" class="nav-link">Our Services</a>

                <a href="/register" class="nav-link">Get in touch</a>

            </div>
        </div>
    </div>
</div>