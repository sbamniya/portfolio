<script lang="ts">
	import TitleAndSubtitle from './../../../comopnents/title-and-subtitle/index.svelte';
	import StudyCard from './study-card.svelte';
	import CaseStudyImage from './../../../assets/images/case-study-1.svg';

	const CaseStudies = [
		{
			image: CaseStudyImage,
			counter: 1,
			title: 'Bakery Landing Page Design',
			description:
				'when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged.',
			button: {
				text: '',
				onClick: () => {}
			}
		},
		{
			image: CaseStudyImage,
			counter: 2,
			title: 'Bakery Landing Page Design',
			description:
				'when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged.',
			button: {
				text: '',
				onClick: () => {}
			}
		},
		{
			image: CaseStudyImage,
			counter: 3,
			title: 'Bakery Landing Page Design',
			description:
				'when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged.',
			button: {
				text: '',
				onClick: () => {}
			}
		},
		{
			image: CaseStudyImage,
			counter: 4,
			title: 'Bakery Landing Page Design',
			description:
				'when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged.',
			button: {
				text: '',
				onClick: () => {}
			}
		},
		{
			image: CaseStudyImage,
			counter: 5,
			title: 'Bakery Landing Page Design',
			description:
				'when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged.',
			button: {
				text: '',
				onClick: () => {}
			}
		},
		{
			image: CaseStudyImage,
			counter: 6,
			title: 'Bakery Landing Page Design',
			description:
				'when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged.',
			button: {
				text: '',
				onClick: () => {}
			}
		},
		{
			image: CaseStudyImage,
			counter: 7,
			title: 'Bakery Landing Page Design',
			description:
				'when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged.',
			button: {
				text: '',
				onClick: () => {}
			}
		}
	];
</script>

<section class="case-studies py-5">
	<TitleAndSubtitle title="CASE STUDY" subTitle="My Case Studies" />
	{#each CaseStudies as caseStudy, index}
		<StudyCard
			image={caseStudy.image}
			title={caseStudy.title}
			description={caseStudy.description}
			counter={caseStudy.counter}
			imagePlacement={index % 2 === 0 ? 'start' : 'end'}
		/>
	{/each}
</section>

<style scoped lang="scss">
	@import './../../../assets/scss/variable';
</style>
