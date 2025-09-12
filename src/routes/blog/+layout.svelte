<script>
  import { base } from "$app/paths";

    let { children } = $props();

    const posts = [
        "09-10-25"
    ]

</script>

{@render children()}

{#each posts as post}
    <a href="{base}/blog/{post}">{post}</a>
{/each}