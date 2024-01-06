<script lang="ts">
	import TitleAndSubtitle from '../../../components/title-and-subtitle/index.svelte';
</script>

<section class="testimonial-container py-5">
	<TitleAndSubtitle title="TESTIMONIALS" subTitle="What People Says" />
	<div class="pt-5">
		<div id="carouselExampleDark" class="carousel carousel-dark slide" data-bs-ride="carousel">
			<div class="left-background" />
			<div class="right-background" />
			<div class="carousel-inner">
				<div class="carousel-item active" data-bs-interval="10000">
					<div class="slide-section">
						<div class="textSection">
							<img src="/user.jpg" class="image" alt="profile" />
							<p>
								If you want to work with a great team player who is a real coding rock star, then
								look no further. Sonu will get your project to completion with ease while he guides
								his team effortlessly! He has performed excellent in a fast-paced and at times
								chaotic environment. Sonu had no problem delivering multiple exceptional quality
								products with last minute changes from the design team. He did this with a smile on
								his face and a great attitude! He was always eager to solve problems and keep the
								projects moving forward. I hope to work with him again very soon! I cannot say
								enough great things about Sonu!
							</p>
							<h5>Devin Newstead</h5>
							<p>Director of Technology at BidWizer</p>
						</div>
					</div>
				</div>
				<div class="carousel-item" data-bs-interval="2000">
					<div class="slide-section">
						<div class="textSection">
							<img src="/user.jpg" alt="profile" class="image" />
							<p>
								We have been working with Sonu for many years now. He is very reliable. I can always
								trust him to get the job done in a timely and professional manner. Great attention
								to detail.
							</p>
							<h5>Matthew Klynsmith</h5>
							<p>Founder at Cerium Group</p>
						</div>
					</div>
				</div>
				<div class="carousel-item" data-bs-interval="2000">
					<div class="slide-section">
						<div class="textSection">
							<img src="/user.jpg" alt="profile" class="image" />
							<p>
								Sonu was excellent. I worked with him over the course of 4 months as we tweaked
								things on our web applet / website. We did UI changes, added features like a chat
								popout, and even some minute work like fine tuning WebP compression of user images
								to minimize server load / usage and load time. Throughout this whole time, Sonu was
								responsive, courteous, professional, and polite. He kindly listened to any bug fixes
								we had or changes to the work and promptly took care of them. His timeliness,
								responsiveness, and kindness, are rare traits in a developer that are extremely
								important. After dealing with some substandard developers, I know the value of a
								good one. He completely earned this excellent review
							</p>
							<h5>Akash Arora</h5>
							<p>Founder at LitLounge.io</p>
						</div>
					</div>
				</div>
				<div class="carousel-item" data-bs-interval="2000">
					<div class="slide-section">
						<div class="textSection">
							<img src="/user.jpg" alt="profile" class="image" />
							<p>
								It was a pleasure working with Sonu. The project took some time to complete, but
								Sonu was always supportive of the changes required. Definitely recommend him to
								consider for your next UI project!
							</p>
							<h5>Niranjan Patil</h5>
							<p>Founder at Adagrad.ai</p>
						</div>
					</div>
				</div>
				<div class="carousel-item" data-bs-interval="2000">
					<div class="slide-section">
						<div class="textSection">
							<img src="/user.jpg" alt="profile" class="image" />
							<p>
								I worked with Sonu for around 2 years and the skill set that he possess in frontend
								technologies is excellent.Having experience in different frontend frameworks he is
								capable enough to build the base of an application and lead the team through it. His
								focus on code quality is also a skill to be appraised. Having a helpful nature makes
								him the best team player and I really enjoyed working with him. I wish him good luck
								for his new role and journey.
							</p>
							<h5>Jaikant</h5>
							<p>Freelance QA Engineer</p>
						</div>
					</div>
				</div>
				<div class="carousel-item" data-bs-interval="2000">
					<div class="slide-section">
						<div class="textSection">
							<img src="/user.jpg" alt="profile" class="image" />
							<p>
								Sonu and I’ve worked for around 3 years, he is one of the most dedicated software
								professionals I’ve worked with, he is proactive, result-oriented, and responsible
								and is not only a multi-skilled and insightful professional but also an inspiring
								strategist. He has extreme problem-solving skills, he makes sure all the deadlines
								are met and makes sure that whatever project he is working on meets the highest
								standards.
							</p>
							<h5>Chanchal</h5>
							<p>Senior QA Engineer</p>
						</div>
					</div>
				</div>
			</div>
			<button
				class="carousel-control-prev"
				type="button"
				data-bs-target="#carouselExampleDark"
				data-bs-slide="prev"
			>
				<span class="carousel-control-prev-icon" aria-hidden="true" />
				<span class="visually-hidden">Previous</span>
			</button>
			<button
				class="carousel-control-next"
				type="button"
				data-bs-target="#carouselExampleDark"
				data-bs-slide="next"
			>
				<span class="carousel-control-next-icon" aria-hidden="true" />
				<span class="visually-hidden">Next</span>
			</button>
		</div>
	</div>
</section>

<style scoped lang="scss">
	@import './../../../assets/scss/variable';
	@import './../../../assets/scss/mixins';
	.testimonial-container {
		.image {
			border-radius: 100px;
			height: 100px;
			width: 100px;
		}
		.left-background {
			position: absolute;
			background-color: #fff1ff;
			width: 650px;
			height: 200px;
		}
		.right-background {
			position: absolute;
			width: 171px;
			height: 157px;
			background-image: url(../../../assets/images/Frame.png);
			background-repeat: no-repeat;
			right: 0;
		}
		.slide-section {
			position: relative;
			width: 60%;
			height: auto;
			margin-left: 35%;
			padding: 60px 0px 10px 0px;
			text-align: center;
			.textSection {
				background-color: $white;
				box-shadow: 0px 0px 20px rgba(0, 0, 0, 0.1);
				padding: 60px 10px 10px 10px;
				border-radius: 18px;
				&::after {
					content: '';
					position: absolute;
					background-image: url(../../../assets/images/comma_Left.png);
					background-repeat: no-repeat;
					background-size: contain;
					width: 25px;
					height: 19px;
					left: 30px;
					top: 90px;
				}
				&::before {
					content: '';
					position: absolute;
					background-image: url(../../../assets/images/comma_Right.png);
					background-repeat: no-repeat;
					background-size: contain;
					width: 25px;
					height: 19px;
					right: 30px;
					bottom: 30px;
				}
				img {
					position: absolute;
					top: 10px;
					margin: auto;
					left: 0;
					right: 0;
				}
				p {
					font-weight: 400;
					opacity: 0.5;
					font-size: $font-14;
					padding-bottom: 20px;
					width: 77%;
					margin: auto;
				}
			}
		}
		.carousel-control-prev,
		.carousel-control-next {
			background-color: $primary;
			position: absolute;
			width: 100px;
			height: 70px;
			top: 160px;
			opacity: 1;
		}
		.carousel-control-prev {
			left: 30%;
			border-radius: 10px 0 0 10px;
		}
		.carousel-control-next {
			left: 36%;
			border-radius: 0 10px 10px 0;
		}
		@include mq(sm) {
			.left-background {
				width: 90%;
			}
			text-align: center;
			.slide-section {
				width: 90%;
				margin: auto;
			}
			.carousel-control-prev,
			.carousel-control-next {
				display: inline-flex;
				position: static;
				width: 50px;
				height: 50px;
				padding: 15px;
			}
		}
	}
</style>
