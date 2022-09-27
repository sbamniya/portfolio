<script>
	import ContactMe from '../comopnents/footer/index.svelte';
	import Navbar from '../comopnents/navbar/index.svelte';
	import Meproud from '../pages/home/me-proud/index.svelte';
	import Testimonial from '../pages/home/testimonial/index.svelte';
	import './../assets/scss/_global.scss';
</script>

<div class="main">
	<div class="main-container">
		<Navbar />
		<slot />
	</div>
	<br /> <br />
	<Testimonial />
	<Meproud />
	<ContactMe />
</div>

<style scoped lang="scss">
	.main {
		height: 100vh;
		background: linear-gradient(
			180deg,
			rgba(236, 178, 46, 0.0754) 0%,
			rgba(255, 255, 255, 0.1144) 100%
		);

		.main-container {
			width: 90%;
			margin: auto;
		}
	}
</style>
