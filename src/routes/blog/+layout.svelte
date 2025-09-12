<script>
    let { children } = $props();

    const posts = [
        "09-10-25"
    ]

</script>

{@render children()}

{#each posts as post}
    <a href="blog/{post}">{post}</a>
{/each}