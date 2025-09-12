<script>
    import { fade } from 'svelte/transition';
    import { page } from '$app/state';
    import { resolve } from '$app/paths';

    let { children } = $props();
</script>

<div>
    <a class="title" href="/">pugsrdubs</a>
    <a href={resolve("/")}>home</a>
    <a href={resolve("/about")}>about</a>
    <a href={resolve("/blog")}>blog</a>

    <hr>

    <span>{@render children()}</span>
    
</div>
<footer>site credits or whatever</footer>

<style>
    :global(body) {
        background-image: url("beach-dark.jpeg");
        background-size: cover;
        background-position: center;
        background-repeat: no-repeat;
        height: 100vh;
        margin: 0;
        background-color: rgb(44, 44, 44);
    }
    :global(a, p, li, label) {
        color: white;
        font-family: "Funnel Sans", sans-serif;
        font-optical-sizing: auto;
        font-style: normal;
    }
    :global(h2) {
        color: white;
        text-decoration-line: none;
        font-family: "Funnel Display", sans-serif;
        font-size: 30px;
        font-weight: 800;
        margin-top: 0px;
        margin-bottom: 10px;
    }
    a {
        margin-right: 10px;
    }
    .title {
        text-decoration-line: none;
        font-family: "Funnel Display", sans-serif;
        font-size: 50px;
        font-weight: 800;
        margin-top: 0px;
        margin-bottom: 10px;
    }
    div {
        padding: 30px;
        margin-top: 30px;
        margin-left: auto;
        margin-right: auto;
        width: 600px;
        background-color: rgb(44, 44, 44);
        opacity: 90%;
        /*height: 350px;*/
    }
    footer {
        padding: 10px;
        position: fixed;
        left: 0;
        bottom: 0;
        width: 100%;
        color: rgb(126, 126, 126);
        text-align: center;
    }
</style>