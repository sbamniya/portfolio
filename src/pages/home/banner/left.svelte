<script>
	import HireMe from '../../../components/hireme/index.svelte';
	import DownloadCV from '../../../components/download-cv/index.svelte';
</script>

<section class="main-box">
	<p class="hello-text">Hello I am,</p>
	<h3 class="name">Sonu Bamniya</h3>
	<p class="title">Full Stack JavaScript Developer</p>
	<p class="description">
		I am a seasoned JavaScript Full Stack Developer with over 8 years of experience, specializing in
		creating exceptional web applications. My passion lies in crafting innovative solutions that
		blend seamless user experiences with robust backend architecture.
	</p>
	<HireMe />
	<DownloadCV>Download CV</DownloadCV>
</section>

<style scoped lang="scss">
	@import './../../../assets/scss/variable';

	.main-box {
		font-family: $poppins-regular;
		.hello-text {
			color: $primary;
			font-size: $font-18;
		}

		.name {
			text-transform: uppercase;
			font-family: $poppins-semibold;
			font-size: 62px;
		}

		.title {
			color: $green;
			font-size: $font-22;
		}
		.description {
			line-height: 26px;
			color: rgba($color: $black, $alpha: 0.5);
			font-size: $font-16;
		}
	}
</style>
