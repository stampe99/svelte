<script>
	import { time } from './stores.js';
	
	let showModal = false;
	export let url;

	let kitty = false;

	const handleMouseenter = () => kitty = true;
	const handleMouseleave = () => kitty = false;

	// Klocka
	const formatter = new Intl.DateTimeFormat('en', {
		hour12: true,
		hour: 'numeric',
		minute: '2-digit',
		second: '2-digit'
	});

</script>

<main>
	<h2 class="welcome">{url}</h2>
	<p>this is my first <a href="https://svelte.dev/">Svelte </a> web app.</p>
	<p>{formatter.format($time)}</p>
</main>

<!--
<button on:click="{() => showModal = true}">
	show modal
</button>
-->
<!--
<svelte:body
	on:mouseenter={handleMouseenter}
	on:mouseleave={handleMouseleave}
/>

<img
	class:curious={kitty}
	alt="Kitten wants to know what's going on"
	src="https://svelte.dev/tutorial/kitten.png"
>
-->
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
	/*
	img {
		position: absolute;
		left: 0;
		bottom: -60px;
		transform: translate(-80%, 0) rotate(-30deg);
		transform-origin: 100% 100%;
		transition: transform 0.4s;
	}

	.curious {
		transform: translate(-15%, 0) rotate(0deg);
	}
	*/
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
