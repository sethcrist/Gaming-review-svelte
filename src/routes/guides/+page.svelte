<!--fetching data-->
<script>
    import {onMount} from "svelte";

    /**
     * @typedef {Object} Guide
     * @property {number} userId - the User ID
     * @property {number} it - weird id
     * @property {string} title - The title of the guide
     * @property {string} body - The body content of the guide
     */

    // {
    //     "userId": 1,
    //     "it": 1,
    //     "title": "are or do repels provide blacked out except option criticizes",
    //     "body": "because he also accepts\nundertakes the consequences of refusal and when\nhe criticizes the trouble so that the whole\nof our things are but they are the matter will happen to the architect"
    // },

    /** @type {Guide[]} */
    let guides = [];

    onMount(async () => {
        /** @type {Response} */
        const res = await fetch('https://jsonplaceholder.typicode.com/posts');
        if (res.ok) {
            guides = await res.json();
            console.log(res);
        }
    });
</script>

<div class="guides">
    <ul>
        {#each guides as guide}
           <li>
               <a href="/">{guide.title}</a>
           </li>
        {/each}
    </ul>
</div>

<!--<footer>-->
<!--</footer>-->

<style>
    .guides {
        margin-top: 20px;
    }
    ul {
        list-style-type: none;
        padding: 0;
    }
    a {
        display: inline-block;
        margin-top: 10px;
        padding: 10px;
        border: 1px dotted rgba(255, 255, 255, 0.2);
    }
</style>