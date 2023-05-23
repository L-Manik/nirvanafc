<script lang="ts">
	import Section from '$components/Section.svelte';
	import book from 'svelte-awesome/icons/book';
	import music from 'svelte-awesome/icons/music';
	import cogs from 'svelte-awesome/icons/cogs';
	import user from 'svelte-awesome/icons/user';
</script>

<div class="readable-area">
	<div class="header">
		<div class="header-text">
			<h1 style="font-size: 3rem">Nirvana</h1>
			<p>Biggest Band of the 90s</p>
		</div>
		<img
			alt="Nirvana Logo"
			class="avatar"
			src="data:image/png;base64,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"
		/>
	</div>

	<div class="content">
			<Section iconData={user} title="Members">
				<p>Learn more about the members of the band.</p>
			</Section>
		<Section iconData={book} title="Brief History">
			<ul>
				<li>
					2011-2014
					<br />
					&emsp; Bikini Bottom High School
				</li>
				<li>
					2014-2018
					<br />
					&emsp; New Kelp City Culinary College
				</li>
			</ul>
		</Section>
		<Section iconData={music} title="Albums">
			<ul>
				<li>Bleach (1989)</li>
				<li>Nevermind (1991)</li>
				<li>In Utero (1993)</li>
			</ul>
		</Section>
		<Section iconData={cogs} title="Present">
			<ul>
				<li>What are the members of Nirvana doing now?</li>
			</ul>
		</Section>
	</div>
</div>

<style>
	h1 {
		font-family: 'peralta';
	}

	ul {
		list-style-type: none;
	}

	li {
		display: flex;
		flex-direction: row;
		align-items: center;
		justify-content: space-between;
	}

	.header-text {
		text-align: center;
		flex: 1;
		margin-right: 16px;
	}

	.readable-area {
		display: flex;
		flex-direction: column;
		background-color: #030302;
		margin: 0 5%;
		height: 100%;
	}

	.header {
		padding: 16px;
		display: flex;
		flex-direction: column-reverse;
		align-items: center;
		border-bottom: 2px solid black;
		text-decoration: none;
		color: #000000;
	}

	.content {
		display: grid;
		grid-template-columns: repeat(1, minmax(0, 1fr));
		gap: 32px;
		padding: 32px 32px;
	}

	img {
		width: 128px;
		height: 128px;
		border: 4px solid #000000;
		border-radius: 100%;
	}

	@media (min-width: 600px) {
		.header {
			flex-direction: row;
		}

		.header-text {
			text-align: end;
		}

		.content {
			grid-template-columns: repeat(2, minmax(0, 1fr));
		}

		.readable-area {
			margin: 0 10%;
		}
	}

	@media (min-width: 1000px) {
		.readable-area {
			margin: 0 20%;
		}
	}
</style>
