<script>;
	  import snarkdown from 'snarkdown'

let post1 = `
# Detta är en blogg-post med markdown
## [Markdown](https://github.com/mattcone/markdown-guide/blob/master/cheat-sheet.md)

## Detta är en underrubrik
### Detta är en underrubrik med fler nivåer
- Detta är en lista

---
~~oj~~ \n

This text is _bold_
`

</script>

<main>
    <h2 class="welcome">Blog</h2>
    <p>välkommen till bloggen</p>
</main>

<div class="posts">
	<div class="card">
		<div class="post">
			{@html snarkdown(post1)}
		</div>
	</div>
</div>
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

	.posts {
		text-align: center;
	}

	.card {
		background-color: darkgrey;
		width: 35em auto;
		height: 50px auto;
		margin: 20px auto;
		border-radius: 10px;
		padding: 20px;
		box-shadow: 0px 0px 10px #000;
		background-size: 50%;
	}
</style>
