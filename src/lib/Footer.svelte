<script>
	import { page } from '$app/stores';
	import { get } from 'svelte/store';
	import Ssblogo from './icons/Ssblogo.svelte';
	import Navlogo from './icons/Navlogo.svelte';

</script>

<footer>
	<div class="row">
		Brukt av
		<Ssblogo />og <Navlogo />
	</div>
	<span>
		<span style="text-decoration: underline">Snakk med oss</span> om Nais kan passe hos dere</span
	>
</footer>

<style>
	footer {
		font-size: 1.2rem;
		background-color: #fcc6c67f;
		padding: 1rem;
		text-align: center;
		margin-top: auto;
		min-height: 100px;
	}
	.row {
		display: flex;
		align-items: center;
		justify-content: center;
	}
</style>
