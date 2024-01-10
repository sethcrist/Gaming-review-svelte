<script>
    import Title from "$lib/title/+page.svelte"
    import '../lib/styles/global.css'
</script>

<header>
    <Title title="Korvo Gaming Guides" />
</header>

    <main>
        <!-- Page content -->
        <slot>

        </slot>
    </main>

<footer>
    <p>Copyright 2024 Korvo Gaming guide</p>
</footer>

<style>
    header {
        display: flex;
        justify-content: center;
    }
    main {
        max-width: 960px;
        margin: 20px auto;
    }
    footer {
        text-align: center;
    }
</style>