<script>
	import Card from '../../../components/card/index.svelte';
	import ServiceOne from '../../../assets/images/service-1.svg';
	import TitleAndSubtitle from '../../../components/title-and-subtitle/index.svelte';
	const Services = [
		{
			image: ServiceOne,
			title: 'Full Stack Development',
			description:
				'Proficient in React, Angular, Vue.js, Node.js, and Express.js for responsive UIs and high-performance APIs. A collaborative problem solver, adept at contributing across the development lifecycle. Adaptable to industry trends, committed to delivering top-notch solutions.'
		},
		{
			image: ServiceOne,
			title: 'Frontend Development',
			description:
				"Passionate about crafting innovative, responsive web interfaces and high-performance APIs. A collaborative problem solver committed to delivering top-notch solutions and staying abreast of industry trends. Let's elevate your projects together."
		},
		{
			image: ServiceOne,
			title: 'Backend Development',
			description:
				"Specializing in crafting seamless user experiences and robust backend architectures. A collaborative problem solver, dedicated to delivering top-notch solutions and staying current with industry trends. Let's discuss how my expertise can elevate your projects."
		}
	];
</script>

<section class="service-details py-5" id="services">
	<TitleAndSubtitle title="Services" subTitle="Check My Services" />
	<div class="row services-container pt-5">
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
