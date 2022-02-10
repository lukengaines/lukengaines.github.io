<script>
  import Fa from 'svelte-fa'
  import { faLinkedin } from '@fortawesome/free-brands-svg-icons'
</script>
<main>
	<header>
		<h1>Luke Gaines</h1>
		<div id="links">
			<a href="/">
				<Fa icon={faLinkedin} />
			</a>
		</div>
	</header>
	<div id="vid">
	</div>
</main>

<style>
	#links {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}
	#links > a {
		color: #ffebe4;
		text-decoration: none;
		font-size: 2em;
	}
	#vid {
		background-color: #7e7c7c;
		flex: 1;
		width: 80vw;
		min-height: 80vh;
		border: 5px solid #7e7c7c
	}
	main {
		padding: 1em;
		margin: 0 auto;
		display: flex;
		flex-direction: column;
		align-items: center;
	}
	header {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		flex: 1;
		width: 100%;
		margin-bottom: 1em;
	}
	h1 {
		color: #ffebe4;
		font-size: 4em;
		font-weight: 100;
		margin-top: 0em;
		margin-bottom: 0em;
	}

	@media (max-width: 640px) {
		main {
			max-width: none;
		}
		h1 {
		font-size: 3em;
		}
	}
</style>