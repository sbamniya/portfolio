<script lang="ts">
	import TitleAndSubtitle from './../../../comopnents/title-and-subtitle/index.svelte';
	import PortfolioImage from './../../../assets/images/portfolio-1.svg';
	const PortfolioItems = [
		{
			image: PortfolioImage
		},
		{
			image: PortfolioImage
		},
		{
			image: PortfolioImage
		},
		{
			image: PortfolioImage
		}
	];
</script>

<section class="portfolio-container py-5" id="portfolio">
	<TitleAndSubtitle title="PORTFOLIO" subTitle="People Lie Work Don't" />
	<div class="row">
		{#each PortfolioItems as item}
			<div class="col-sm-6 col-xs-12">
				<img src={item.image} alt="" class="w-100" />
			</div>
		{/each}
	</div>
</section>

<style scoped lang="scss">
	.portfolio-container {
		.row {
			row-gap: 20px;
			margin-top: 50px;
		}
	}
</style>
