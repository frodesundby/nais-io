<script lang="ts">
	import Header from "$lib/Header.svelte"
</script>

<div class="main bg-gray-100">
	<div class="absolute inset-0 bg-gray-100 bg-gradient-to-b from-gray-100 via-white to-white">
		<svg
			class="pointer-events-none absolute left-1/2 -translate-x-1/2 top-0 w-full min-w-[80rem] h-auto"
			width="1171"
			height="241"
			viewBox="0 0 1171 241"
			fill="none"
		>
			<g opacity=".175" filter="url(#filter0_f)">
				<path
					d="M731.735 -179.55C596.571 -157.762 516.36 -74.1815 552.576 7.13199C588.793 88.4455 727.724 136.701 862.887 114.913C998.051 93.1247 1078.26 9.54454 1042.05 -71.769C1005.83 -153.082 866.898 -201.337 731.735 -179.55Z"
					fill="url(#paint0_linear)"
				></path>
				<path
					d="M378 114.106C520.489 114.106 636 45.8883 636 -38.2623C636 -122.413 520.489 -190.63 378 -190.63C235.511 -190.63 120 -122.413 120 -38.2623C120 45.8883 235.511 114.106 378 114.106Z"
					fill="url(#paint1_linear)"
				></path>
			</g>
			<defs>
				<filter
					id="filter0_f"
					x="0"
					y="-310.63"
					width="1170.74"
					height="550.775"
					filterUnits="userSpaceOnUse"
					color-interpolation-filters="sRGB"
				>
					<feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
					<feBlend mode="normal" in="SourceGraphic" in2="BackgroundImageFix" result="shape"
					></feBlend>
					<feGaussianBlur stdDeviation="60" result="effect1_foregroundBlur"></feGaussianBlur>
				</filter>
				<linearGradient
					id="paint0_linear"
					x1="567.5"
					y1="1.03997"
					x2="1029.02"
					y2="64.6468"
					gradientUnits="userSpaceOnUse"
				>
					<stop stop-color="#001AFF"></stop>
					<stop offset="1" stop-color="#6EE5C2"></stop>
				</linearGradient>
				<linearGradient
					id="paint1_linear"
					x1="155"
					y1="-11.0234"
					x2="511.855"
					y2="-162.127"
					gradientUnits="userSpaceOnUse"
				>
					<stop stop-color="#FFC83A"></stop>
					<stop offset="0.504191" stop-color="#FF008A"></stop>
					<stop offset="1" stop-color="#6100FF"></stop>
				</linearGradient>
			</defs>
		</svg>
	</div>
	
	<Header />

	<div class="content">
		<div class="left">
			<h3>
				En offentlig,
				<br />offentlig sky,
				<br />for det offentlige
			</h3>
			<h2>
				Plattformen der Nav har tatt steget fra <br /><em>fire</em> leveranser <em>per år</em>
				<br />til <em>tusenvis</em> av deploys <em>per uke</em>
			</h2>
		</div>
		<div class="banner_img">
			<figure><img class="img_responsive" src="banner_img.png" /></figure>
		</div>
	</div>
</div>

<style>
    @import url('https://fonts.googleapis.com/css?family=Poppins:100,100i,200,200i,300,300i,400,400i,500,500i,600,600i,700,700i,800,800i,900,900i');
	.main {
		font-size: 14px;
		font-family: 'Poppins', sans-serif;
		line-height: 1.80857;
		font-weight: normal;
		height: 100vh;
		text-align: center;
		@font-face {
			font-family: 'Poppins';
			src: url('https://fonts.googleapis.com/css?family=Poppins:100,100i,200,200i,300,300i,400,400i,500,500i,600,600i,700,700i,800,800i,900,900i');
		}
	}
	.main .content {
		display: flex;
		flex-direction: row;
	}
    .banner_img {
        width: 900px;
    }
    .img_responsive {
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
	.to-white {
		--tw-gradient-to: #fff var(--tw-gradient-to-position);
	}
	.via-white {
		--tw-gradient-to: rgb(255 255 255 / 0) var(--tw-gradient-to-position);
		--tw-gradient-stops: var(--tw-gradient-from), #fff var(--tw-gradient-via-position),
			var(--tw-gradient-to);
	}
	.from-gray-100 {
		--tw-gradient-from: #f1f2f9 var(--tw-gradient-from-position);
		--tw-gradient-to: rgb(241 242 249 / 0) var(--tw-gradient-to-position);
		--tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to);
	}
	.bg-gradient-to-b {
		background-image: linear-gradient(to bottom, var(--tw-gradient-stops));
	}
	.bg-gray-100 {
		--tw-bg-opacity: 1;
		background-color: rgb(241 242 249 / var(--tw-bg-opacity));
	}
	*,
	::before,
	::after {
		--tw-border-spacing-x: 0;
		--tw-border-spacing-y: 0;
		--tw-translate-x: 0;
		--tw-translate-y: 0;
		--tw-rotate: 0;
		--tw-skew-x: 0;
		--tw-skew-y: 0;
		--tw-scale-x: 1;
		--tw-scale-y: 1;
		--tw-pan-x: ;
		--tw-pan-y: ;
		--tw-pinch-zoom: ;
		--tw-scroll-snap-strictness: proximity;
		--tw-gradient-from-position: ;
		--tw-gradient-via-position: ;
		--tw-gradient-to-position: ;
		--tw-ordinal: ;
		--tw-slashed-zero: ;
		--tw-numeric-figure: ;
		--tw-numeric-spacing: ;
		--tw-numeric-fraction: ;
		--tw-ring-inset: ;
		--tw-ring-offset-width: 0px;
		--tw-ring-offset-color: #fff;
		--tw-ring-color: rgb(59 130 246 / 0.5);
		--tw-ring-offset-shadow: 0 0 #0000;
		--tw-ring-shadow: 0 0 #0000;
		--tw-shadow: 0 0 #0000;
		--tw-shadow-colored: 0 0 #0000;
		--tw-blur: ;
		--tw-brightness: ;
		--tw-contrast: ;
		--tw-grayscale: ;
		--tw-hue-rotate: ;
		--tw-invert: ;
		--tw-saturate: ;
		--tw-sepia: ;
		--tw-drop-shadow: ;
		--tw-backdrop-blur: ;
		--tw-backdrop-brightness: ;
		--tw-backdrop-contrast: ;
		--tw-backdrop-grayscale: ;
		--tw-backdrop-hue-rotate: ;
		--tw-backdrop-invert: ;
		--tw-backdrop-opacity: ;
		--tw-backdrop-saturate: ;
		--tw-backdrop-sepia: ;
	}


</style>
