<script>
	import Button from '../button/index.svelte';
	import mailIcon from '../../assets/images/icons/mail.svg';
	import addressIcon from '../../assets/images/icons/address.svg';
	import phoneIcon from '../../assets/images/icons/phone.svg';
</script>

<section class="contact-us-container pt-5">
	<div class="row main-container">
		<div class="col-sm-7 col-xs-12">
			<div class="Contact-section pt-0 pt-sm-5">
				<div class="px-0 px-sm-5 ">
					<h3>Contact us</h3>
					<span>
						We are committed to processing the information in order to contact you and talk about
						your project.
					</span>
				</div>
				<div class="Contact-detail">
					<p><img src={mailIcon} alt="" />example@teamwebflow.com</p>
					<p><img src={addressIcon} alt="" />4040 Lekki Summit Suite 402 Lake Manchester City</p>
					<p><img src={phoneIcon} alt="" />+44 123 777 5401</p>
				</div>
			</div>
		</div>
		<div class="col-sm-5 col-xs-12">
			<div class="Form-section">
				<form>
					<div class="mb-3">
						<input type="text" class="form-control input-box" placeholder="Name" />
					</div>
					<div class="mb-3">
						<input type="email" class="form-control input-box" placeholder="Email" />
					</div>
					<div class="mb-3">
						<input type="text" class="form-control input-box" placeholder="Website" />
					</div>
					<div class="mb-3">
						<textarea class="form-control" rows="7" placeholder="Message" />
					</div>
					<Button>Submit</Button>
				</form>
			</div>
		</div>
		<section>
			<div class="footer-section">
				<div class="row">
					<div class="col-sm-4">
						<div class="footer-leftside">
							<h2>Sonu</h2>
							<p>is simply dummy text of the printing and typesetting industry. Lorem Ipsum</p>
						</div>
					</div>
					<div class="col-sm-8">
						<div class="footer-rightside">
							<ul>
								<h6>EXPLORE</h6>
								<li><a href="/">SUPPORTS</a></li>
								<li><a href="/">ABOUT US</a></li>
								<li><a href="/">BLOG</a></li>
							</ul>
							<ul>
								<h6>LEGAL</h6>
								<li><a href="/">TERMS OF USE</a></li>
								<li><a href="/">PRIVACY POLICY</a></li>
							</ul>
							<ul>
								<h6>SOCIALS</h6>
								<li><a href="/">TWITTER</a></li>
								<li><a href="/">LINKEDIN</a></li>
								<li><a href="/">INSTAGRAM</a></li>
							</ul>
						</div>
					</div>
				</div>
			</div>
		</section>
	</div>
	<div class="footer-bottom" />
</section>

<style scoped lang="scss">
	@import './../../assets/scss/variable';
	@import './../../assets/scss/mixins';

	.contact-us-container {
		background: linear-gradient(
			180deg,
			rgba(236, 178, 46, 0.0754) 0%,
			rgba(255, 255, 255, 0.1144) 100%
		);
		.main-container {
			width: 90%;
			margin: auto;
			.Contact-section {
				span {
					font-size: $font-14;
					color: #999;
					margin-bottom: 20px;
				}
				.Contact-detail {
					padding-top: 40px;
					img {
						margin-right: 15px;
						width: 20px;
					}
					p {
						font-size: $font-16;
						color: #999;
					}
				}
			}
			.Form-section {
				.input-box {
					height: 70px;
				}
			}
		}

		.footer-section {
			padding: 100px 0;
			@include mq(sm) {
				padding: 30px 0;
			}
			.footer-leftside {
				h2 {
					color: $primary;
					font-size: 50px;
					font-family: $logo-font;
				}
				p {
					color: #999;
					font-size: $font-12;
				}
			}
			.footer-rightside {
				display: flex;
				justify-content: space-around;
				@include mq(sm) {
					display: block;
				}
				ul {
					padding: 0;
					list-style: none;
					h6 {
						padding-bottom: 20px;
					}

					li {
						font-size: $font-18;
						padding-bottom: 20px;
						a {
							color: #999;
							text-decoration: none;
							font-size: $font-14;
						}
					}
				}
			}
		}
		.footer-bottom {
			background-color: $primary;
			height: 50px;
		}
	}
</style>
