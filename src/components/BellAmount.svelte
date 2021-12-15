<script>
    let blls = 420
</script>

<main>
    <div class="container">
        <!-- Value -->
        <div class="container__top">You have</div>

        <!-- Label -->
        <div class="container__bot">{blls} $BLL</div>
    </div>
</main>

<style>
    .container {
        /* Center the content */
        align-items: center;
        display: inline-flex;
        flex-direction: column;
    }

    .container__top {
        font-size: 1rem;
        font-weight: 500;
        margin-bottom: 5%;
    }

    .container__bot {
        font-size: 2rem;
        font-weight: 300;

        /* Uppercase the label */
        /* text-transform: uppercase; */
    }
</style>
