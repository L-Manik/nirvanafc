<script lang="ts">
	import Icon from 'svelte-awesome';
	import type { IconType } from 'svelte-awesome/components/Icon.svelte';

	export let iconData: IconType;
	export let title: string;
</script>

<div class="container">
	<div 
	class="section-title">
		<Icon data={iconData} />
		{title}
	</div>
	<slot />
</div>

<style>
	.section-title {
		display: flex;
		align-items: center;
		gap: 16px;
		background-color: #135de7;
		border-left: 4px solid #053ca3;
		color: black;
		padding: 8px 16px;
		text-transform: UPPERCASE;
		font-weight: 500;
	}
	.container {
		display: flex;
		flex-direction: column;
		gap: 16px;
		border: 2px solid #053ca3;
		padding: 16px
	}
</style>
