<script>
    export let name = '';
    export let description = '';
    export let url = '';
</script>

<div class="tool-link">
    <h2>{name}</h2>
    <p>{description}</p>
    <a href={url} target="_blank">Visit</a>
</div>

<style>
    .tool-link {
        border: 1px solid #ddd;
        padding: 1rem;
        margin-bottom: 1rem;
    }
    .tool-link a {
        color: #0066cc;
    }
</style>