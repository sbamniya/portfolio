<script>
	import './../assets/scss/_global.scss';
	import Navbar from '../comopnents/navbar/index.svelte';
</script>

<div class="main">
	<div class="main-container">
		<Navbar />
		<slot />
	</div>
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
