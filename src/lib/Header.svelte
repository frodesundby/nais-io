<script>
	import { page } from '$app/stores';
	import { get } from 'svelte/store';

	const isActive = (/** @type {string} */ path) => get(page).url.pathname === path;
</script>

<div class="row">
	<a href="/" class="logo">nais.io</a>
	<nav class="navigation navbar navbar-expand-md navbar-dark">
		<ul class="navbar-nav mr-auto">
			<li class="nav-item">
				<a class="nav-link" href="https://nais.io/blog/">Artikler</a>
			</li>
			<li class="nav-item">
				<a class="nav-link" href="https://docs.nais.io">Dokumentasjon</a>
			</li>
			<li class="nav-item">
				<a class="nav-link" href="/logg" class:isActive={isActive('/logg')}>Logg</a>
			</li>
			<!-- <li class="nav-item">
				<a class="nav-link" href="/status" class:isActive={isActive('/status')}>Status</a>
			</li> -->
			<li class="nav-item">
				<a class="nav-link" href="mailto:nais@nav.no">Kontakt oss</a>
			</li>
		</ul>
	</nav>
	<!-- <div class="logo"/> -->
	<a class="github-link nav-link" href="https://github.com/nais"
		><img class="github" src="github-mark.svg" alt="nais github" />
	</a>
</div>

<style>
	.github {
		height: 30px;
	}
	.nav-link.github-link {
		text-transform: none;
		display: flex;
		align-items: center;
		gap: 8px;
	}
	.row {
		font-size: 14px;
		font-family: 'Poppins', sans-serif;
		line-height: 1.80857;
		font-weight: normal;
		text-align: center;
	}
	.nav-link.isActive {
		background-color: rgb(249, 182, 167);
	}
	.logo {
		text-decoration: none;
		font-weight: 600;
		font-size: 2rem;
		margin-top: 12px;
		color: #f0390f;
		margin-left: 100px;
	}
	.logo:hover {
		text-decoration: underline;
	}
	.nav-link {
		padding: 15px 20px;
		color: #2b2b2b;
		font-size: 17px;
		line-height: 20px;
		font-weight: 400;
		border-radius: 30px;
		text-transform: uppercase;
		text-decoration: none !important;
	}

	.nav-link:hover {
		background-color: #f0390f;
		color: #fff;
	}
	.navigation.navbar {
		float: right;
		padding: 0;
	}
	.navbar {
		position: relative;
		display: -ms-flexbox;
		display: flex;
		-ms-flex-wrap: wrap;
		flex-wrap: wrap;
		-ms-flex-align: center;
		align-items: center;
		-ms-flex-pack: justify;
		justify-content: space-between;
		padding: 0.5rem 1rem;
	}
	.navbar-nav {
		display: -ms-flexbox;
		display: flex;
		-ms-flex-direction: row;
		flex-direction: row;
		padding-left: 0;
		margin-bottom: 0;
		list-style: none;
	}
	li {
		display: list-item;
		text-align: -webkit-match-parent;
		unicode-bidi: isolate;
	}
	.row {
		display: flex;
		flex-direction: row;
		align-items: center;
		align-content: center;
		justify-content: space-between;
	}
</style>
