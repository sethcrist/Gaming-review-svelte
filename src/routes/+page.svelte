<script>
    let title = "Gaming Guide for the inept."

    const updateTitle = () => {
        title = "something different"
    }
</script>

<div class="index">
    <h2>{title}</h2>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aperiam asperiores aspernatur assumenda autem,
        delectus dicta doloribus ducimus eius enim eveniet facere fugiat illo impedit iste laboriosam laborum magnam
        natus nobis non perspiciatis quae qui quo recusandae rem tempora totam ut vel veniam vero voluptas. Eligendi,
        ipsa, nihil! Accusantium assumenda delectus eum ipsa necessitatibus nulla pariatur, quos, tempore tenetur unde vero.</p>

    <button on:click={updateTitle}>Change title</button>

<!--binding values to input fields-->
    <input type="text" bind:value={title}>

    <a href="/guides">View Guides</a>
    <a href="/about">About</a>

</div>

<style>
    .index {
        text-align: center;
        display: block;
        margin: 20px auto;
    }

</style>