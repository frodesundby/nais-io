<script>
	import Brukere from '$lib/Brukere.svelte';
	import Glance from '$lib/Glance.svelte';
	import Navlogo from '$lib/icons/Navlogo.svelte';
</script>

<div class="content">
	<div class="left">
		<!-- <h3>
		En offentlig,
		<br />offentlig sky,
		<br />for utviklere i det offentlige
	</h3> -->
		<h3>
			En plattform <br />laget av <Navlogo style="width:100; height:2rem; color:#f0390f;" /><br />
			for å gi fart og flyt <br />til utviklerne av <br />det offentlige Norge
		</h3>
		<h2>
			Vi mener at det skal være lett å gjøre rett.<br /> Utviklerne bør kunne fokusere det som betyr
			noe - å lage gode applikasjoner.
		</h2>
		<!-- <h2 style="line-height: 2rem; max-width: 580px;">
			Nais er en applikasjonsplattform og verktøykasse for å hjelpe utviklere med å
			<em>levere</em>.
			<div style="padding-top: 16px">Laget av Nav, tilgjengelig for det offentlige.</div>
		</h2> -->
		<a class="cta" href="https://docs.nais.io">Lær mer om Nais</a>
	</div>
	<div class="banner_img">
		<figure>
			<img class="img_responsive" src="multicloud.png" alt="tegneseriesky med norsk banner" />
		</figure>
	</div>
</div>
<Brukere />
<div class="glances">
	<Glance heading="Utrulling og attestering" logoUrl="deploy.png">
		Nais har Github Actions som bygger, tester, inspiserer, signerer og deployer applikasjonen.
		Når du pusher koden, bygges et image og aplikasjonens bibliotek og avhengigheter kartlegges for å lage en attestert innholdsfortegnelse (<a href="FIXME">SBOM</a>).
		Med image og SBOM på plass kan applikasjonen deployes til et miljø.
	</Glance>
	<Glance heading="Automatisert infrastruktur" logoUrl="infra.png">
		Du spesifiserer hva applikasjonen din har behov for, så sørger Nais for å sette det opp og gi deg det du trenger for å bruke det; 
		trenger du en database, så settes det opp av Nais og applikasjonen din får brukernavn, passord og tilgang på nettverksnivå ut av boksen.
	</Glance>
	<Glance heading="Innsikt og oversikt" logoUrl="monitoring.png">
		.
	</Glance>
</div>

<style>
	.glances {
		display: flex;
		gap: 2rem;
	}
	.content {
		min-width: 1432px;
		width: 1432px;
		display: flex;
		flex-direction: row;
	}
	.cta {
		display: inline-block;
		margin-top: 30px;
		padding: 15px 20px;
		color: white;
		font-size: 17px;
		line-height: 20px;
		font-weight: 400;
		border-radius: 30px;
		text-transform: uppercase;
		text-decoration: none !important;
		background-color: #f0390f;
	}
	.cta:hover {
		background-color: rgb(250, 132, 105);
	}
	.banner_img {
		width: 900px;
	}
	.img_responsive {
		margin-top: 20%;
		width: 82%;
		height: auto;
	}
	.content .left {
		left: 0;
		right: 0;
		text-align: left;
		position: inherit;
		min-width: 500px;
	}
	.left h3 {
		padding-top: 60px;
		font-size: 3.5rem;
		line-height: 85px;
		color: #2b2b2b;
		font-weight: bold;
	}
	.left h2 {
		letter-spacing: 0;
		font-weight: normal;
		position: relative;
		padding: 0;
		font-weight: normal;
		line-height: normal;
		color: #111111;
		margin: 0;
	}
</style>
