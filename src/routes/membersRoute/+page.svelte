<script lang="ts">
	import Section from '$components/Section.svelte';
	import book from 'svelte-awesome/icons/book';
	import music from 'svelte-awesome/icons/music';
	import cogs from 'svelte-awesome/icons/cogs';
	import user from 'svelte-awesome/icons/user';
	import Members from '$lib/components/Members.svelte';
</script>

<div class="readable-area">
	<header>
		<h1>Meet the Members of Nirvana!</h1>
	</header>
	<Members iconData={user} title="Kurt Cobain"> </Members>
</div>

<style>
	body {
		margin: 0;
		padding: 0;
	}

	.readable-area {
		padding: 5px;
		max-width: 960px;
		width: 95%;
		margin: 20px auto;
	}

	header {
		padding: 0 15px;
		text-align: center;
		font-size: 21px;
	}

	.columns {
		display: flex;
		flex-flow: row wrap;
		justify-content: center;
		margin: 5px 0;
	}

	.memberbox {
		flex: 1;
		border: 1px solid;
		margin: 5px;
		padding: 16px;
		justify-content: center;
		transition: 0.3s;
		background: black;
	}

	@media screen and (max-width: 980px) {
		.columns .memberbox{
			margin-bottom: 5px;
			flex-basis: 40%;
		}
	}
</style>
