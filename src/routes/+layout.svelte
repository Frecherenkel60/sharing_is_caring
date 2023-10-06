<script lang="ts">
	import '../app.postcss';

	// Floating UI for Popups
	import { arrow, autoUpdate, computePosition, flip, offset, shift } from '@floating-ui/dom';
	import { AppShell, storePopup } from '@skeletonlabs/skeleton';
	// Import components
	import LandingPageFooter from '$lib/landingPage/LandingPageFooter.svelte';
	import LandingPageHeader from '$lib/landingPage/LandingPageHeader.svelte';

	// Set the default options for all popups
	storePopup.set({ computePosition, autoUpdate, flip, shift, offset, arrow });
</script>

<AppShell>
	<svelte:fragment slot="header">
		<LandingPageHeader />
	</svelte:fragment>
	<slot />
	<svelte:fragment slot="footer">
		<LandingPageFooter />
	</svelte:fragment>
</AppShell>
