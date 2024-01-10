<script>
    export let title = "Korvo Gaming"
</script>

<div class="title">
    <img src="/gaming.jpg" alt="site icon">
    <h1>{title}</h1>
</div>

<style>
    .title {
        display: flex;
    }
    .title img {
        display: inline-block;
        border-radius: 50px;
        width: 75px;
        height: 75px;
        margin-top: 40px;
    }
    .title h1 {
        margin-left: 5px;
    }
    h1 {
        display: inline-block;
        margin-top: 60px;
        font-size: 2em;
        /*color: linear-gradient(to right, blue, purple)*/
    }
</style>