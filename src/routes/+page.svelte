<div class="hero">
	<h1>Hi There.</h1>
</div>

<style>
	div.hero {
		display: flex;
		align-items: center;
		justify-content: center;
	}
	h1 {
		background: radial-gradient(
			circle,
			#f48fb1 0%,
			#ce93d8 20%,
			#b2ebf2 40%,
			#a5d6a7 60%,
			#b39ddb 100%
		);
		-webkit-background-clip: text;
		color: transparent;
		background-size: 400%;
		animation: gradient 10s linear infinite alternate;
		font-size: 8rem;
	}

  h1:hover {
		animation: gradient 4s linear infinite alternate;
		font-size: 8rem;
	}

	@keyframes gradient {
		0% {
			background-position: 0%;
		}
		100% {
			background-position: 100%;
		}
	}
</style>
