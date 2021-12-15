<script>
  import Head from "./components/Head.svelte";
  import WalletConnect from "./components/WalletConnect.svelte";
  
</script>

<Head />

<main>
  <h1>Turnip Token</h1>
  <WalletConnect />
</main>

<style>
  :global(body) {
    font-family: "Press Start 2P";
    text-align: center;
    font-size: 12px;
    color: #f0e117;
    background: rgb(247, 247, 182);
  }

  h1 {
    margin-top: 75px;
    margin-bottom: 100px;
    font-size: 4em;
    font-weight: 400;
    color: #55fc76;
  }

  a {
    text-decoration: underline;
    color: beige;
  }
  a:hover {
    color: #ffcf22;
  }

  @media (max-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
