<script lang="ts">
	import Header from '$lib/Header.svelte';
	import Footer from '$lib/Footer.svelte';
</script>

<div class="main">
	<Header />

	<div class="gradient"></div>

	<div class="content">
		<div class="left">
			<h3>
				En offentlig,
				<br />offentlig sky,
				<br />for utviklere i det offentlige
			</h3>
			<h2 style="line-height: 2rem; max-width: 580px;">
				Nais er en applikasjonsplattform og verktøykasse for å hjelpe utviklere med å
				<em>levere</em>.
				<div style="padding-top: 16px">Laget av Nav, tilgjengelig for det offentlige.</div>
			</h2>
			<a class="cta" href="https://docs.nais.io">Lær mer om Nais</a>
		</div>
		<div class="banner_img">
			<figure><img class="img_responsive" src="multicloud.png" /></figure>
		</div>
	</div>

	<Footer />
</div>

<style>
	.main::before {
		position: absolute;
		content: '';
		height: 300px;
		width: 500px;
		left: 50%;
		transform: translate(-75%, -60%);
		border-radius: 100%;
		background: linear-gradient(to right, #ffc73a22, #ff008822, #6200ff22);
		filter: blur(100px);
	}
	.main::after {
		position: absolute;
		content: '';
		height: 300px;
		width: 500px;
		left: 50%;
		transform: translate(0, -60%);
		border-radius: 100%;
		background: linear-gradient(to right, #001aff22, #6ee5c222);
		filter: blur(100px);
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
	@import url('https://fonts.googleapis.com/css?family=Poppins:100,100i,200,200i,300,300i,400,400i,500,500i,600,600i,700,700i,800,800i,900,900i');
	.main {
		font-size: 14px;
		font-family: 'Poppins', sans-serif;
		line-height: 1.80857;
		font-weight: normal;
		height: 100vh;
		text-align: center;
		display: flex;
		flex-direction: column;

		background-color: rgb(241 242 249);

		@font-face {
			font-family: 'Poppins';
			src: url('https://fonts.googleapis.com/css?family=Poppins:100,100i,200,200i,300,300i,400,400i,500,500i,600,600i,700,700i,800,800i,900,900i');
		}
	}
	.main .content {
		display: flex;
		flex-direction: row;
		flex-grow: 1;
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
	}
	.left {
		margin-left: 10%;
		min-width: 500px;
	}
	.left h3 {
		padding-top: 60px;
		font-size: 70px;
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
	.absolute {
		position: absolute;
	}
</style>
