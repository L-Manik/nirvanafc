<script lang="ts">
	import Icon from 'svelte-awesome';
	import type { IconType } from 'svelte-awesome/components/Icon.svelte';

	export let iconData: IconType;
	export let title: string;
</script>

<div class="container">
	<div class="section-title">
		<Icon data={iconData} />
		{title}
	</div>
	<slot />
</div>

<style>
	.section-title {
		border-radius: 5px;
		display: flex;
		align-items: center;
		gap: 16px;
		background-color: #135de7;
		border-left: 8px solid #053ca3;
		color: white;
		padding: 8px 16px;
		text-transform: UPPERCASE;
		font-weight: 500;
		font: "Nirvana";
	}
	.container {
		border-radius: 25px;
		display: flex;
		flex-direction: column;
		gap: 16px;
		padding: 16px;
		box-shadow: 20px 20px 50px rgba(0, 0, 0, 0.5);
		background: rgba(225, 225, 225, 0.1);
		overflow: hidden;
		border-top: 1px solid rgba(24, 148, 243, 0.377);
		border-left: 1px solid rgba(24, 148, 243, 0.377);
		backdrop-filter: blur(5px);
		transition: 0.5s;
	}

    @font-face {
    font-family: 'Nirvana';
    font-style: normal;
    font-weight: normal;
    src: local('Nirvana'), url('NIRVANA.woff') format('woff');
    }
	.container:hover {
		transform:scale(1.1);
	}
</style>
