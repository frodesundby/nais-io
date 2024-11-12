<script>
	import Navlogo from '$lib/icons/Navlogo.svelte';
</script>

<div class="hero">
	<div class="content">
		<h2>
			En plattform laget av <Navlogo />
			for å gi fart og flyt til utviklerne av det offentlige Norge
		</h2>
		<p>
			Vi mener at det skal være lett å gjøre rett. Utviklerne bør kunne fokusere det som betyr noe -
			å lage gode applikasjoner.
		</p>
		<a class="cta" href="https://docs.nais.io">Lær mer om Nais</a>
	</div>
	<img class="cloud" src="multicloud.png" alt="" />
</div>

<style>
	.hero {
		padding: 3rem 0.5rem;
		display: flex;
		flex-direction: column;
		align-items: center;
		gap: 2rem;
	}
	.content {
		display: flex;
		flex-direction: column;
		gap: 1rem;
	}
	.cloud {
		width: 50%;
	}
</style>
