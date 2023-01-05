<script lang="ts" context="module">
    import "the-new-css-reset/css/reset.css"
    import "../../src/global.css"
</script>

<div class="outer-container">
    <main>
        <slot />
    </main>
    <aside>
        <p>this is side bar</p>
    </aside>
</div>

<style>
    .outer-container {
        padding: 1rem;
        display: grid;
        grid-template-columns: 0.7fr 0.3fr;
        column-gap: 5rem;
    }
</style>