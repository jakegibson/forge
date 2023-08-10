<script lang="ts">
	import engleadership from '$lib/assets/engleadership.webp';
	import mlops from '$lib/assets/mlops.webp';
	import kubernetes from '$lib/assets/utahkubernetes.webp';
</script>

<div class="container h-full mx-auto">
	<h1 class="h1">Upcoming Utah Dev Events</h1>
	<h1 class="h1">Forge Meetups</h1>
	<div class="grid md:grid-cols-3 gap-4">
		<a href="https://www.meetup.com/engineering-leadership-utah/" class="card overflow-hidden">
			<header>
				<img alt="Engineering leadership meetup header of a mountain" src={engleadership} />
			</header>
			<div class="card-body">
				<p>
					Engineering Leadership is a meetup for engineering leaders to share ideas, learn from each
					other, and build a community of practice around leadership.
				</p>
			</div>
			<div class="card-footer">
				<button class="btn btn-sm variant-primary">Learn More</button>
			</div>
		</a>

		<a href="https://www.meetup.com/engineering-leadership-utah/" class="card overflow-hidden">
			<header>
				<img alt="Engineering leadership meetup header of a mountain" src={mlops} />
			</header>
			<div class="card-body">
				<p>
					Engineering Leadership is a meetup for engineering leaders to share ideas, learn from each
					other, and build a community of practice around leadership.
				</p>
			</div>
			<div class="card-footer">
				<button class="btn btn-sm variant-primary">Learn More</button>
			</div>
		</a>

		<a href="https://www.meetup.com/engineering-leadership-utah/" class="card overflow-hidden">
			<header>
				<img
					class="aspect-video"
					alt="Engineering leadership meetup header of a mountain"
					src={kubernetes}
				/>
			</header>
			<div class="card-body">
				<p>
					Engineering Leadership is a meetup for engineering leaders to share ideas, learn from each
					other, and build a community of practice around leadership.
				</p>
			</div>
			<div class="card-footer">
				<button class="btn btn-sm variant-primary">Learn More</button>
			</div>
		</a>
	</div>
	<h1 class="h1">Lost Sheep Meetups</h1>
	<div class="grid md:grid-cols-3 gap-4">
		<a href="https://www.meetup.com/engineering-leadership-utah/" class="card overflow-hidden">
			<header>
				<img alt="Engineering leadership meetup header of a mountain" src={engleadership} />
			</header>
			<div class="card-body">
				<p>
					Engineering Leadership is a meetup for engineering leaders to share ideas, learn from each
					other, and build a community of practice around leadership.
				</p>
			</div>
			<div class="card-footer">
				<button class="btn btn-sm variant-primary">Learn More</button>
			</div>
		</a>

		<a href="https://www.meetup.com/engineering-leadership-utah/" class="card overflow-hidden">
			<header>
				<img alt="Engineering leadership meetup header of a mountain" src={mlops} />
			</header>
			<div class="card-body">
				<p>
					Engineering Leadership is a meetup for engineering leaders to share ideas, learn from each
					other, and build a community of practice around leadership.
				</p>
			</div>
			<div class="card-footer">
				<button class="btn btn-sm variant-primary">Learn More</button>
			</div>
		</a>

		<a href="https://www.meetup.com/engineering-leadership-utah/" class="card overflow-hidden">
			<header>
				<img
					class="aspect-video"
					alt="Engineering leadership meetup header of a mountain"
					src={kubernetes}
				/>
			</header>
			<div class="card-body">
				<p>
					Engineering Leadership is a meetup for engineering leaders to share ideas, learn from each
					other, and build a community of practice around leadership.
				</p>
			</div>
			<div class="card-footer">
				<button class="btn btn-sm variant-primary">Learn More</button>
			</div>
		</a>
	</div>
</div>

<style lang="postcss">
	figure {
		@apply flex relative flex-col;
	}
	figure svg,
	.img-bg {
		@apply w-64 h-64 md:w-80 md:h-80;
	}
	.img-bg {
		@apply absolute z-[-1] rounded-full blur-[50px] transition-all;
		animation: pulse 5s cubic-bezier(0, 0, 0, 0.5) infinite, glow 5s linear infinite;
	}
	@keyframes glow {
		0% {
			@apply bg-primary-400/50;
		}
		33% {
			@apply bg-secondary-400/50;
		}
		66% {
			@apply bg-tertiary-400/50;
		}
		100% {
			@apply bg-primary-400/50;
		}
	}
	@keyframes pulse {
		50% {
			transform: scale(1.5);
		}
	}
</style>
