<script>
    import Modal from './Modal.svelte';
    import { onMount } from 'svelte';
</script>

<main>
    <h2 class="welcome">About</h2>
</main>

<style>
    main {
        text-align: center;
        padding: 1em;
        max-width: 240px;
        margin: 0 auto;
    }

    h2 {
        font-size: 50px;
    }

    .welcome {
        text-transform: lowercase;
        background-image: linear-gradient(
            -225deg,
            #231557 0%,
            #44107a 29%,
            #ff1361 67%,
            #fff800 100%
        );
        background-size: auto auto;
        background-clip: border-box;
        background-size: 200% auto;
        color: #fff;
        background-clip: text;
        -text-fill-color: transparent;
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        animation: textclip 2s linear infinite;
        display: inline-block;
        transform: rotate(-1deg);
    }
</style>
