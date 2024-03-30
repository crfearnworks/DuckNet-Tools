<script>
    export let tool;
</script>

<div class="tool-link">
    <h3>{tool.name}</h3> {tool.description} <a href={tool.url} target="_blank">Visit</a>
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