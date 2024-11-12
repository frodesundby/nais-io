<script lang="ts">
	export let heading: string;
	export let logoUrl: string;
</script>

<div class="glance">
	<div class="icon">
		<img src={logoUrl} alt="glance logo" />
	</div>
	<div class="content">
		<h2>{heading}</h2>
		<p><slot /></p>
	</div>
</div>

<style>
	.glance {
		min-width: 450px;
		max-width: 450px;
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
		min-width: 330px;
		h2 {
			margin: 0;
			text-align: start;
			vertical-align: top;
			font-size: 1.5rem;
			font-weight: bold;
		}
		text-align: left;
	}
</style>
