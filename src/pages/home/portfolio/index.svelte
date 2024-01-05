<script lang="ts">
	import TitleAndSubtitle from '../../../components/title-and-subtitle/index.svelte';
	import BidWizer from './../../../assets/images/bidwizer.png';
	import ZestHRM from './../../../assets/images/zesthrm.png';

	const PortfolioItems = [
		{
			image: ZestHRM,
			link: 'https://www.zesthrm.com/'
		},
		{
			image: BidWizer,
			link: 'https://www.bidwizer.com/'
		}
	];
</script>

<section class="portfolio-container py-5" id="portfolio">
	<TitleAndSubtitle title="PORTFOLIO" subTitle="People Lie Work Don't" />
	<div class="row">
		{#each PortfolioItems as item}
			<div class="col-sm-6 col-xs-12 cursor-pointer">
				<a href={item.link} target="_blank">
					<img src={item.image} alt="" class="w-100 image" />
				</a>
			</div>
		{/each}
	</div>
</section>

<style scoped lang="scss">
	.portfolio-container {
		.row {
			row-gap: 20px;
			margin-top: 50px;
			.cursor-pointer {
				cursor: pointer;
			}

			.image {
				height: 100%;
				border-radius: 10px;
			}
		}
	}
</style>
