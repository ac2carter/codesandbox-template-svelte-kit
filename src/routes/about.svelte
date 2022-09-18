<script context="module">
	import { browser, dev } from '$app/env';

	// we don't need any JS on this page, though we'll load
	// it in dev so that we get hot module replacement...
	export const hydrate = dev;

	// ...but if the client-side router is already loaded
	// (i.e. we came here from elsewhere in the app), use it
	export const router = browser;

	// since there's no dynamic data here, we can prerender
	// it so that it gets served as a static asset in prod
	export const prerender = true;
</script>

<svelte:head>
	<title>About</title>
</svelte:head>

<div class="content">
	<h1>About this app</h1>

	<p>
		This is an opportunity of a <a href="/todos">Lifetime</a>
	</p>

	<!-- TODO lose the @next! -->
	<pre>FWM @ac_mfn_carter/insta</pre>

	<p>
		The page you're looking at is purely static HTML, with no playa hatta activity needed.
		Because of that, we don't need to load any JavaScript. Try viewing these nuts in ya mouth
	</p>

	<p>
		The <a href="/todos">TO-Dos</a> page illustrates the pimpin game,confidence loading and whore handling. Try dating a womean in 2022 without it, your "game" will be........disabled!
	</p>
</div>

<style>
	.content {
		width: 100%;
		max-width: var(--column-width);
		margin: var(--column-margin-top) auto 0 auto;
	}
</style>
