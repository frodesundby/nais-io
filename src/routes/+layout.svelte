<script lang="ts">
	import Header from '$lib/Header.svelte';
	import '../styles/app.css';
</script>

<div class="main">
		<Header />
		<slot />
		<!-- <Footer /> -->
</div>

<style>
	.main {
		font-size: 14px;
		line-height: 1.80857;
		font-weight: normal;
		min-height: 100vh;
		text-align: center;
		display: flex;
		flex-direction: column;
		background-color: rgb(241 242 249);
        justify-items: center;
        align-items: center;
	}

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
	:global(.page) {
		margin: 0 auto 0 auto;
		min-width: 1000px;
		max-width: 1432px
	}
	@media (max-width: 1464px) {
		:global(.page) {
			padding: 0 2rem;
		}
	}
</style>
