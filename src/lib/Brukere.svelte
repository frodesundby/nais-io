<script>
	import Navlogo from './icons/Navlogo.svelte';
	import SsblogoFull from './icons/SsblogoFull.svelte';
</script>

<div class="section">
	<div>Nais er brukt av utviklingsteam hos</div>
	<div class="users">
		<Navlogo />
		<SsblogoFull />
	</div>
	<div>
		<a class="mail" href="mailto:nais@nav.no">Snakk med oss</a> om Nais kan passe hos dere
	</div>
</div>

<style>
	.section {
		font-size: 1.5rem;
		padding-block: 4rem;
		padding-inline: 4vw;
		max-width: var(--content-max-width);
		text-align: center;
		display: grid;
		gap: 1rem;
	}
	.users {
		font-size: 3rem;
		display: flex;
		flex-wrap: wrap;
		column-gap: 2rem;
		row-gap: 1rem;
		align-items: center;
		justify-content: center;
	}
	.mail {
		color: var(--color-primary);
		font-weight: bold;
	}
</style>
