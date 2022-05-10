<script>

</script>

<main>
    <h2 class="welcome">contact</h2>
    <p>kontakta support</p>
    <p>-</p>
    <div class="contact-card">
        <div class="title">
            <div class="title-header">
                <h3>kontakta oss</h3>
            <div class="title-body">
                <p>
                    <span>e-post:</span>
                    <span>
                        <a href="mailto: e@gmail.com">mail@here.com</a>
                    </span>
                </p>
            </div>
    </div>
</main>

<style>
    main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}

	h2 {
		font-size: 50px;
	}

	p {
		font-size: 25px;
	}

	:global(body) {
		overflow: hidden;
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
