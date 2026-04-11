<script>
  import { base } from "$app/paths";

</script>
<h2>check out the:</h2>

<div>
    <a href="{base}/about">about</a>
    <a href="{base}/projects">projects</a>
    <a href="{base}/blog">blog</a>
</div>

<style>
    div {
        text-align: center;
        margin-top: 40px;
        margin-bottom: 20px;
    }
    a {
        background-color: rgb(25, 25, 25);
        margin-left: 10px;
        margin-right: 10px;
        padding: 30px;
        border: white;
        border-radius: 5px;
        transition: all 300ms;
        text-decoration: none;
        font-weight: normal;
        font-size: 20px;
    }
    a:hover {
        background-color: rgb(25, 25, 25);
        filter: drop-shadow(0px 0px 5px #ffffff);
    }
    a:active {
        background-color: rgb(60, 60, 60);
    }
</style>