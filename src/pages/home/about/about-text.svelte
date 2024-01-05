<script>
	import HireMe from '../../../components/hireme/index.svelte';
	import DownloadCV from '../../../components/download-cv/index.svelte';
	import ExperienceIcon from './../../../assets/images/icons/experience.svg';
	import ProjectIcon from './../../../assets/images/icons/projects.svg';
	import SupportIcon from './../../../assets/images/icons/support.svg';

	const aboutMetaDetails = [
		{
			icon: ExperienceIcon,
			title: '8 years+',
			subTitle: 'Experience'
		},
		{
			icon: ProjectIcon,
			title: '10+',
			subTitle: 'Projects'
		}
	];
</script>

<section class="about-section" id="about">
	<div class="about-text-container">
		<p class="sup-text">A bit</p>
		<h3 class="title">About Me</h3>
		<p class="text">
			I am a seasoned JavaScript Full Stack Developer with over 8 years of experience, specializing
			in creating exceptional web applications. My passion lies in crafting innovative solutions
			that blend seamless user experiences with robust backend architecture. Throughout my career, I
			have mastered a wide range of front-end and back-end technologies, including React, Angular,
			Vue.js, Node.js, and Express.js. These skills enable me to design responsive and intuitive
			user interfaces and develop high-performance APIs and server-side logic. Being an enthusiastic
			problem solver, I thrive in collaborative environments where I can contribute my expertise
			across the entire development lifecycle. From conceptualizing project architectures to
			deployment and maintenance, I take pride in delivering top-notch solutions. Constantly staying
			up-to-date with the latest industry trends and best practices, I continuously seek to expand
			my skill-set and incorporate cutting-edge technologies. This adaptability allows me to lead
			and collaborate effectively within diverse development teams, fostering creativity and
			innovation.
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
