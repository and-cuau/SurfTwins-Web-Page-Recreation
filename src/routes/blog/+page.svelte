<script>
	const blogPosts = [
		{
			name: `Morocco's Best Surf Packages | Surf Camp & Lessons in Essaouira | SurfTwins`,
			description:
				'Nestled along the stunning Atlantic coastline of Morocco, Essaouira is a surfer’s paradise known for its consistent waves, vibrant culture, and breathtaking scenery. At Surftwins Essaouira, we’ve crafted the perfect surf getaway for wave enthusiasts of all levels. Whether you’re a beginner catching your first wave or an advanced surfer seeking thrilling breaks, our surfing experiencesEssaouira are designed to deliver an unforgettable experience.',
			link: 'http://...',
			img: 'https://cdn.prod.website-files.com/617c00c2cfd67cd06be8ba9f/679dff39c511a3291e961bc5_surftwins%20style.jpg'
		},
		{
			name: `Surftwins Essaouira exploring the Ultimate Surf and Kite Destination: Sidi Kaouiki, Essaouira, Morocco`,
			description:
				'Nestled along the stunning Atlantic coastline of Morocco, Essaouira is a surfer’s paradise known for its consistent waves, vibrant culture, and breathtaking scenery. At Surftwins Essaouira, we’ve crafted the perfect surf getaway for wave enthusiasts of all levels. Whether you’re a beginner catching your first wave or an advanced surfer seeking thrilling breaks, our surfing experiencesEssaouira are designed to deliver an unforgettable experience.',
			link: 'http://...',
			img: 'https://cdn.prod.website-files.com/617c00c2cfd67cd06be8ba9f/679ce5ffc06156aeb0a156c0_surftwins%20kite%20surf.jpg'
		},
		{
			name: `Surftwins Essaouira Is It Possible to Learn to Surf After 30? Absolutely!`,
			description:
				'Nestled along the stunning Atlantic coastline of Morocco, Essaouira is a surfer’s paradise known for its consistent waves, vibrant culture, and breathtaking scenery. At Surftwins Essaouira, we’ve crafted the perfect surf getaway for wave enthusiasts of all levels. Whether you’re a beginner catching your first wave or an advanced surfer seeking thrilling breaks, our surfing experiencesEssaouira are designed to deliver an unforgettable experience.',
			link: 'http://...',
			img: 'https://cdn.prod.website-files.com/617c00c2cfd67cd06be8ba9f/679ce5ffc06156aeb0a156c0_surftwins%20kite%20surf.jpg'
		}
	];
</script>


<section class="hero-homepage">
	<div class="container">
		<h1 class="home-h1">SurfTwins Blog</h1>
	</div>
</section>


<section id="posts">
	{#each blogPosts as blog}
		<div class="post">
			<img src={blog.img} alt="" />
			<div class="text-wrap">
				<div class="name">{blog.name}</div>
				<p class="no-margin">{blog.description}</p>
				<a href={blog.link}>Read more</a>
			</div>
		</div>
	{/each}
</section>

<style>

	@import url('https://fonts.googleapis.com/css2?family=Nunito:wght@200..1000&family=Red+Hat+Display:ital,wght@0,300..900;1,300..900&display=swap');

	* {
	font-family: 'Red Hat Display', sans-serif;
	}

	
	#posts {
		display: flex;
		flex-direction: column;
		/* align-items: left; */
		align-items: flex-start;
		gap: 60px;
		width: 100%;
		margin-top: 60px;
		flex-wrap: wrap;
	}
	img {
		/* max-width: 200%;
		max-height: 100%;
		width: 100px;
		height: 50px; */
		width: 50vw;
		align-self: center;
	}
	.post {
		max-width: 300px;
		display: inline-flex;
		 /* align-items: center; */
		gap: 130px;
		/* height: 900px; */
		/* //flex-grow: 1; Makes all items expand equally */
		/* add padding */
		border-bottom: 1px solid #A9A9A9; /* 1px thick, solid, black line */
	

	}

	.text-wrap{
		/* padding-left: 100px;
		padding-right: 100px */
		height: 900px;
		width: 800px;
		flex: 1; /* Allows it to expand to take available space */
		min-width: 200px; /* Ensures it doesn’t get too narrow */
	}

	.no-margin {
		margin-bottom: 0;
		margin-left: 0;
	}

	p {
		margin-bottom: 10px;
		margin-left: px;
		font-size: 16px;
		line-height: 160%;
		width: 100%
	}
	.name {
		font-size: 32px;
		font-weight: bold;
		width: 100%;
		margin: 10px 0;
	}

	.hero-homepage {
		background-image: linear-gradient(#fdfcfc00 67%, #fdfcfc99 94%), linear-gradient(96deg, #21212133 22%, #0000),
		url(https://cdn.prod.website-files.com/617c00c2cfd67cd06be8ba9f/679dff39c511a3291e961bc5_surftwins%20style.jpg);
		background-size: cover;
		height: 70dvh;
	}
</style>
