<script>
	import ContactMe from '../comopnents/footer/index.svelte';
	import Navbar from '../comopnents/navbar/index.svelte';
	import './../assets/scss/_global.scss';
</script>

<div class="main">
	<div class="main-container">
		<Navbar />
		<slot />
	</div>
	<br /> <br />
	<ContactMe />
</div>

<style scoped lang="scss">
	.main {
		height: 100vh;

		.main-container {
			width: 90%;
			margin: auto;
		}
	}
</style>
