<script lang="ts">
	import TitleAndSubtitle from './../../../comopnents/title-and-subtitle/index.svelte';
	import slackImage from '../../../assets/images/slack logo.svg';
</script>

<section class="meproud-container py-5">
	<TitleAndSubtitle title="OUR CLIENTS" subTitle="Who Makes Me Proud" />
	<div class="container">
		<div class="row">
			<div class="col-sm-3 col-xs-6 text-center my-4 my-sm-5">
				<img src={slackImage} alt="slackImage" />
			</div>
			<div class="col-sm-3 col-xs-6 text-center my-4 my-sm-5">
				<img src={slackImage} alt="slackImage" />
			</div>
			<div class="col-sm-3 col-xs-6 text-center my-4 my-sm-5">
				<img src={slackImage} alt="slackImage" />
			</div>
			<div class="col-sm-3 col-xs-6 text-center my-4 my-sm-5">
				<img src={slackImage} alt="slackImage" />
			</div>
		</div>
	</div>
</section>

<style scoped lang="scss">
	@import './../../../assets/scss/variable';
</style>
