<script>
	import Navlogo from './icons/Navlogo.svelte';
	import SsblogoFull from './icons/SsblogoFull.svelte';
</script>

<div class="brukere">
	<div class="row">
		Nais er brukt av utviklingsteam hos
		<div class="logos">
				<Navlogo style="height: 50; width:110; color:#333" />
				<SsblogoFull style="height: 50; color: #333" />
		</div>
	</div>
	<span style="text-decoration: underline">Snakk med oss</span> om Nais kan passe hos dere
</div>

<style>
	.logos {
		min-height: 70px;
        min-width: 800px;
		margin: 20px 0;
		display: flex;
		justify-content: center;
        align-items: center;
        gap: 4rem;
	}
	.brukere {
		font-size: 1.2rem;
		padding: 1rem;
		text-align: center;
		min-height: 100px;
        margin-top: 100px;
		margin-bottom: 100px;
	}
	.row {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}
</style>
