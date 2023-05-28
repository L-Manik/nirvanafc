<svelte:head>
	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous" />
	<link
		href="https://fonts.googleapis.com/css2?family=Open+Sans:wght@300;400;500&family=Peralta&display=swap"
		rel="stylesheet"
	/>
	<meta name="viewport" content="width=device-width, initial-scale=1" />
	<script src="https://kit.fontawesome.com/d0c488930b.js" crossorigin="anonymous"></script>
</svelte:head>

<slot />

<style>
	:global(*) {
		margin: 0;
		padding: 0;
		font-family: 'Open Sans';
		color: #e3e5f2
	}
	:global(html, body) {
		width: 100%;
		height: 100%;
		background: linear-gradient(45deg, #101223, #09104d);
	}
	:global(a) {
		text-decoration: none;
	}

	@font-face {
    font-family: 'Nirvana';
    font-style: normal;
    font-weight: normal;
    src: local('Nirvana'), url('fonts/NIRVANA.TTF') format('TTF');
    }
</style>
