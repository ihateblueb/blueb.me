<script>
	import Footer from './Footer.svelte'
</script>

<div class="content">
	<div class="topbox">
		<div class="contentbox">
			<div>
				<h1 class="hi">hi! i'm harper</h1>
				<h3 class="shortabout">you may also know me as ihateblueb or blueb</h3>
			</div>
			<div>
				<h4>my background</h4>
				<p>
					i've been into the internet since the first learned about it. one of
					my first ever websites i made in 2015 when i was in second or third
					grade on wix.
				</p>
				<p>
					after that, i learned basic html and css from my dad and continued to
					learn more about making websites. later on in 2018 i was introduced to
					node.js from wanting to make a discord bot. since then, i've done a
					lot around node and javascript, and it's a huge part of what i do now.
				</p>
			</div>
			<div>
				<h4>my projects</h4>
				<p>
					i'm currently an admin alongside my friend kurbiis for our server,
					Orchid. check it out at <a href="https://orchidmc.me/"
						>https://orchidmc.me/</a
					>!
				</p>
				<p>
					i'm also working on a mastodon client which has support for
					glitch-soc, chuckya, and other fork features. check it out at <a
						href="https://github.com/ihateblueb/aster"
						>https://github.com/ihateblueb/aster</a
					>.
				</p>
				<p>
					there's also a cli program i made for interacting with the cobalt api.
					it's the first project i wrote in rust so its kind of messy, but you
					can check it out on <a href="https://github.com/ihateblueb/cobalt-cli"
						>https://github.com/ihateblueb/cobalt-cli</a
					>.
				</p>
			</div>
			<div>
				<h4>my socials</h4>
				<p>i love the fediverse! i have two accounts related to me on it:</p>
				<span class="socialsGroup">
					<div class="socialsFedi">
						<img src="/skeeter.png" alt="wetdry.world mascot" />
						<a href="https://wetdry.world/@ihateblueb">
							@ihateblueb@wetdry.world
						</a>
					</div>
					<div class="socialsFedi">
						<img src="/eepyzone.png" alt="eepy.zone logo" />
						<a href="https://eepy.zone/@blueb"> @blueb@eepy.zone </a>
					</div>
				</span>
				<p>
					i'm also on discord at @ihateblueb if you need something quicker, feel
					free to add me! a lot of my projects are also on github, which you can
					see at <a href="https://github.com/ihateblueb"
						>https://github.com/ihateblueb</a
					>.
				</p>
			</div>
			<Footer />
		</div>
	</div>
</div>

<style>
	.hi {
		color: var(--txt1);
	}
	.shortabout {
		color: var(--txt2);
	}
	.topbox {
		display: flex;
		flex-direction: column;
		align-items: center;
	}
	.content {
		margin: 40px 20px 20px 20px;
	}
	.socialsGroup {
		display: block;
		margin-bottom: 10px !important;
	}
	@keyframes wee {
		0% {
			rotate: 0deg;
		}
		100% {
			rotate: 720deg;
		}
	}
	.socialsFedi img:hover {
        transition: 1s;
        
		animation-name: wee;
		animation-duration: 1s;
		animation-iteration-count: infinite;

        scale: 150%;
	}
	.socialsFedi {
		display: flex;
		align-items: center;
        transition: 1s;

		margin-bottom: 5px !important;
		padding: 2px 5px 2px 5px;

		background-color: #6364ff45;
		width: fit-content;

		border-radius: 7px;

		& img {
			height: 19px;
			margin-right: 5px;
			margin-top: 2px;
			margin-bottom: 2px;
		}
		& a {
			text-decoration: none;
			color: var(--txt1);
		}
	}
	.contentbox {
		max-width: 750px;

		& div {
			margin-bottom: 25px;

			& h4 {
				color: var(--txt1);
				margin-bottom: 10px;
			}
			& p {
				color: var(--txt2);

				& a {
					color: var(--accent1);
				}
			}
			& p:not(:last-child) {
				margin-bottom: 10px;
			}
		}
	}
</style>
