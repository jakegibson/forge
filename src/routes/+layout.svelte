<script lang="ts">
	// The ordering of these imports is critical to your app working properly
	import '../theme.postcss';
	// If you have source.organizeImports set to true in VSCode, then it will auto change this ordering
	import '@skeletonlabs/skeleton/styles/skeleton.css';
	// Most of your app wide CSS should be put in this file
	import '../app.postcss';
	import { AppShell, AppBar } from '@skeletonlabs/skeleton';
	import logo from '$lib/assets/forge-icon.png';
</script>

<!-- App Shell -->
<AppShell>
	<svelte:fragment slot="header">
		<!-- App Bar -->
		<AppBar>
			<svelte:fragment slot="lead">
				<img alt="Forge Foundation Logo. Flame" style="height:60px" src={logo} />

				<strong class="text-xl">Forge Utah Foundation</strong>
			</svelte:fragment>
			<svelte:fragment slot="trail">
				<a
					class="btn btn-sm variant-ghost-surface"
					href="https://join.slack.com/t/forgeutah/shared_invite/zt-pietaeqb-HetfD2OIzn1RHtDtV~CH5g"
					target="_blank"
					rel="noreferrer"
				>
					Slack
				</a>
				<a
					class="btn btn-sm variant-ghost-surface"
					href="https://www.meetup.com/pro/forge-utah/"
					target="_blank"
					rel="noreferrer"
				>
					Meetups
				</a>
				<a
					class="btn btn-sm variant-ghost-surface"
					href="https://twitter.com/ForgeUtah"
					target="_blank"
					rel="noreferrer"
				>
					Twitter
				</a>
				<a
					class="btn btn-sm variant-ghost-surface"
					href="https://github.com/forgeutah"
					target="_blank"
					rel="noreferrer"
				>
					GitHub
				</a>
			</svelte:fragment>
		</AppBar>
	</svelte:fragment>
	<!-- Page Route Content -->
	<slot />
</AppShell>
