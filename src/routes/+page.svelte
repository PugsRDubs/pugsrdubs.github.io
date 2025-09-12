<script>
  import { base } from "$app/paths";

</script>
<h2>check out the:</h2>

<div>
    <a href="{base}/about">about</a>
    <a href="{base}/blog">blog</a>
</div>

<style>
    div {
        text-align: center;
        margin-top: 40px;
        margin-bottom: 20px;
    }
    a {
        font-weight: bold;
        margin-left: 10px;
        margin-right: 10px;
        padding: 30px;
        border-radius: 5px;
        transition: all 300ms;
    }
    a:hover {
        background-color: rgb(25, 25, 25);
        filter: drop-shadow(7px 7px #0a0a0a);
    }
    a:active {
        background-color: rgb(60, 60, 60);
    }
</style>