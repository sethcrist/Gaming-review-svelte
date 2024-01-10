

<header>
    <nav>
        <div class="links">
            <a href="/">Home</a>
            <a href="/about">About</a>
            <a href="/guides">Guides</a>
        </div>
    </nav>

</header>

<main>
    <!-- Page content -->
    <slot>

    </slot>
</main>

<style>
    header {
        text-align: center;
    }
    main {
        max-width: 960px;
        margin: 20px auto;
    }
    /*footer {*/
    /*    text-align: center;*/
    /*}*/
    .links {
        padding: 0 50px;
        margin: 0;
    }
    a {
        margin: auto;
        justify-content: center;
        padding: 0 50px 0 50px;
    }
    nav {
        display: flex;
        justify-content: center;
        align-items: center;
        max-width: 960px;
        margin: 0 90px 0 90px;
        padding: 15px;
    }
</style>



