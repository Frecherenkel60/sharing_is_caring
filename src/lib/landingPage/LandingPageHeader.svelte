<script lang="ts">
	import Icon from '@iconify/svelte';
	import { AppBar, LightSwitch } from '@skeletonlabs/skeleton';
</script>

<AppBar gridColumns="grid-cols-3" slotDefault="place-self-center" slotTrail="place-content-end">
	<svelte:fragment slot="lead">
		<Icon icon="mdi-light:share-variant" style="w-8 h-8" />
	</svelte:fragment>
	<h2 class="h2 font-semibold tracking-tighter font-heading-token">Sharing is caring</h2>
	<svelte:fragment slot="trail">
		<LightSwitch />
	</svelte:fragment>
</AppBar>
