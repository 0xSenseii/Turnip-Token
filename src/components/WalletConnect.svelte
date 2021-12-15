<script>
    import BellAmount from "./BellAmount.svelte";
    export let connected;
    function connectWallet() {
        connected = !connected;
    }
</script>

<main>
    {#if connected}
        <BellAmount />
    {:else}
        <kbd class="container" on:click|preventDefault={() => connectWallet()}>
            Connect wallet
        </kbd>
    {/if}
</main>

<style>
    .container {
        /* Background and color */
        background-color: rgba(0, 0, 0, 0.1);
        border-radius: 4px;
        color: rgba(0, 0, 0, 0.7);

        /* Bottom shadow */
        box-shadow: rgba(0, 0, 0, 0.3) 0px -2px 0px inset,
            rgba(0, 0, 0, 0.4) 0px 1px 1px;

        /* Spacing */
        padding: 8px;
    }
</style>
