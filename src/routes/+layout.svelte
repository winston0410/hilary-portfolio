<script lang="ts" context="module">
    import "../specific/global.scss"
	import "@fontsource/noto-sans-hk/400.css";
	import "@fontsource/noto-sans-hk/700.css";
</script>

<div class="outer-container">
    <main>
        <slot />
    </main>
    <aside>
        <p>this is side bar</p>
    </aside>
</div>

<style lang="scss">
    .outer-container {
        padding: 1rem;
        display: grid;
        grid-template-columns: 0.7fr 0.3fr;
        column-gap: 5rem;
    }
</style>