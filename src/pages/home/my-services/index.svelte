<script>
	import Card from './../../../comopnents/card/index.svelte';
	import ServiceOne from '../../../assets/images/service-1.svg';
	import TitleAndSubtitle from './../../../comopnents/title-and-subtitle/index.svelte';
	const Services = [
		{
			image: ServiceOne,
			title: 'Landing Page Design',
			description:
				" is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s"
		},
		{
			image: ServiceOne,
			title: 'Landing Page Design',
			description:
				" is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s"
		},
		{
			image: ServiceOne,
			title: 'Landing Page Design',
			description:
				" is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s"
		}
	];
</script>

<section class="service-details py-5">
	<TitleAndSubtitle title="Services" subTitle="Check My Services" />
	<div class="row services-container">
		{#each Services as service}
			<div class="col-lg-4 col-xs-12">
				<Card image={service.image} title={service.title} description={service.description} />
			</div>
		{/each}
	</div>
</section>

<style scoped lang="scss">
	@import './../../../assets/scss/variable';
</style>
