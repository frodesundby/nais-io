<script lang="ts">
	export let heading: string
	export let logoUrl: string

</script>

<div class="main">
	<div class="glance">
		<div class="icon">
			<img src={logoUrl} alt="glance logo" />
		</div>
		<div class="content">
			<h2>{heading}</h2>
			<p><slot></slot></p>
		</div>
	</div>
</div>

<style>
	.glance {
		min-height: 100px;
		min-width: 200px;
		max-width: 500px;
		display: flex;
		gap: 40px;
	}
	.glance .icon {
		border: 1px solid #000;
		border-radius: 10px;
		padding: 5px;
		min-width: 50px;
		height: 50px;
		img {
			width: 90%;
			height: 90%;
		}
	}
	.glance .content {
		h2 {
			margin: 0;
			text-align: start;
			vertical-align: top;
			font-size: 1.5rem;
			font-weight: bold;
		}
		text-align: left;
	}
	.main {
		z-index: 10;

		width: 100%;
		font-size: 14px;
		line-height: 1.80857;
		font-weight: normal;
		text-align: center;
		display: flex;
		flex-direction: column;
		justify-items: center;
		align-items: center;
		min-height: 300px;
	}

	.main::before {
		position: absolute;
		content: '';
		height: 300px;
		width: 500px;
		left: 90%;
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
		left: 90%;
		transform: translate(0, -60%);
		border-radius: 100%;
		background: linear-gradient(to right, #001aff22, #6ee5c222);
		filter: blur(100px);
	}
</style>
