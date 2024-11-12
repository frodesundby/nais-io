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
	<Glance heading="Utrulling" logoUrl="deploy.png">
		<!-- Nais tar koden din fra <i>push</i> til <i>prod</i> uten nedetid. -->
		<!-- Nais tar koden din fra <i>push</i> til <i>prod</i>. Uten nedetid. -->
		Nais lar deg ta koden din fra <i>push</i> til <i>prod</i><br /> uten nedetid.
		<!-- Nais tar seg av å ta koden din fra <i>push</i> til <i>prod</i> uten nedetid -->
		<!-- Det er også bygget inn støtte for sikkerhetssystemer som identifiserer og varsler om kjente sårbarheter -->
		<!-- Nais bygger, kartlegger avhengigheter, signerer og ruller ut applikasjonen.
		Når du pusher koden, bygges et image og applikasjonens bibliotek og avhengigheter kartlegges for å lage en attestert innholdsfortegnelse (<a href="/">SBOM</a>).
		Med image og SBOM på plass kan applikasjonen rulles ut. -->
	</Glance>
	<Glance heading="Automatisering" logoUrl="infra.png">
		Du sier hva du trenger, så setter Nais opp infrastrukturen automatisk.
		<!-- Du sier hva du trenger, så setter Nais opp infrastrukturen. Automatisk. -->
		<!-- Du spesifiserer hva applikasjonen din har behov for, så sørger Nais for å sette det opp og gi deg det du trenger for å bruke det; 
		trenger du en database, så settes det opp av Nais og applikasjonen din får brukernavn, passord og tilgang på nettverksnivå ut av boksen. -->
	</Glance>
	<Glance heading="Ha oversikt" logoUrl="monitoring.png">
		Ha kontroll på det du har kjørende, hva det koster og hvor godt du utnytter det.
		<!-- Se hva du har, hva det koster og hvor godt du utnytter det. -->
	</Glance>
</div>
<div class="glances">
	<Glance heading="Innsikt" logoUrl="insight.png">
		Verktøyene du trenger for å få innsikt i hvordan systemene dine oppfører seg.
		<!-- Observer hvordan applikasjonen din oppfører seg og få varsler om noe er galt. -->
		<!-- Du ser hvordan applikasjonen din oppfører seg og varsles om noe er galt. -->
		<!-- Se hvordan applikasjonen din oppfører seg i produksjon, og få varsler om noe er galt. -->
	</Glance>
	<Glance heading="Sikkerhet" logoUrl="insurance.png">
		Alt er stengt i utgangspunktet, så du må pirke dine egne hull. Isolasjon er standard og du
		definerer publikum.
		<!-- Du <a href="https://doc.nais.io/workloads/explanations/zero-trust/">definerer publikum</a> for din applikasjon og varsles om du har sårbarheter. -->
	</Glance>
	<!-- <Glance heading="24/7 vakt" logoUrl="pulse.png">
		Du må passe på applikasjonen din, men vi passer på alt annet. 24/7.
	</Glance> -->
	<Glance heading="Et Nais fellesskap" logoUrl="pulse.png">
		Vi er mange som bruker og utvikler Nais, og vi hjelper hverandre.
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
