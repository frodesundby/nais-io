<script lang="ts">
	import Header from '$lib/Header.svelte';
	import '../styles/app.css';

	import amplitude from '@amplitude/analytics-browser';

	const getApiKey = () => {
		if (window.location.href.includes('nais.io')) {
			return '16d1ee2fd894ca2562eeebb5095dbcf0'; // prod
		}
		return '04203d48401492bda4620a74acf85a5b'; // dev
	};

	export const loggInstance = amplitude.init(getApiKey(), {
		serverUrl: 'amplitude.nav.no/collect',
		serverZone: 'EU'
	});
</script>

<Header />
<slot />
