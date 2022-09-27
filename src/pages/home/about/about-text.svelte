<script>
	import HireMe from '../../../comopnents/hireme/index.svelte';
	import DownloadCV from '../../../comopnents/download-cv/index.svelte';
	import ExperienceIcon from './../../../assets/images/icons/experience.svg';
	import ProjectIcon from './../../../assets/images/icons/projects.svg';
	import SupportIcon from './../../../assets/images/icons/support.svg';

	const aboutMetaDetails = [
		{
			icon: ExperienceIcon,
			title: '5 years+',
			subTitle: 'Experience'
		},
		{
			icon: ProjectIcon,
			title: '700+',
			subTitle: 'Projects'
		},
		{
			icon: SupportIcon,
			title: '24/7',
			subTitle: 'Customer Support'
		}
	];
</script>

<section class="about-section">
	<div class="about-text-container">
		<p class="sup-text">A bit</p>
		<h3 class="title">About Me</h3>
		<p class="text">
			I'm a top online marketer and branding expert, I started my career by lauching the popular
			metaverse design, in just a few short years, I built the brand to millions of social media
			followers and websites visitors. I also created award-winning online products with millions of
			dolloars in online sales you want, you never get personalized experiences and they can be
			upwards of $1000 on hour.
		</p>
		<div class="meta-details">
			{#each aboutMetaDetails as meta}
				<div class="meta-card">
					<img src={meta.icon} alt="" />
					<div>
						<div class="meta-title">{meta.title}</div>
						{meta.subTitle}
					</div>
				</div>
			{/each}
		</div>
		<HireMe />
		<DownloadCV />
	</div>
</section>

<style scoped lang="scss">
	@import './../../../assets/scss/variable';
	@import './../../../assets/scss/mixins';
	.about-section {
		padding: 80px 0;
		@include mq(sm) {
			padding: 0;
		}
		.about-text-container {
			font-family: $poppins-regular;
			.sup-text {
				color: $primary;
				text-transform: uppercase;
				font-size: $font-18;
			}
			.title {
				color: rgba($black, 0.81);
				font-size: $font-36;
			}

			.text {
				color: rgba($black, 0.5);
				font-size: $font-16;
				line-height: 26px;
			}

			.meta-details {
				width: 100%;
				display: flex;
				flex-wrap: wrap;
				row-gap: 16px;
				margin: 50px 0;
				.meta-card {
					width: 50%;
					display: flex;
					gap: 12px;
					@include mq(xs) {
						width: 100%;
					}
					.meta-title {
						color: $primary;
						font-size: $font-16;
					}
				}
			}
			img {
				width: 30px;
			}
		}
	}
</style>
