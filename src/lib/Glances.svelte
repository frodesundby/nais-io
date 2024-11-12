<script>
	import Glance from '$lib/Glance.svelte';
</script>

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
</style>
