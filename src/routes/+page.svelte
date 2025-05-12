<script>
	import Hero from '$lib/components/hero.svelte';
	import Column from '$lib/components/column.svelte';
	import Offers from '$lib/components/offers.svelte';
	import Carousel from '$lib/components/carousel.svelte';

	const columns = [
		{
		img: 'https://cdn.prod.website-files.com/617b6f00715044249cb2b8dc/66215985b11980b4ce330153_surftwins%20%20Esaaouira%20.JPG',
		name: 'Discover with surftwins the ultimate surfing destinations in Essaouira Morocco',
		paragraphs: [
			"Looking for the best surfing destination? Look no further than Essaouira Morocco! With warm weather year-round, Morocco is a surfer's paradise.",
			"If you're planning a surf trip, our surf school in Sidi Kaouki, Essaouira, is a must-visit. Essaouira is a beautiful and peaceful city with stunning beaches and incredible waves. Immerse yourself in the sun and water while perfecting your surfing skills.",
			"Join us for a surf lesson, a surf trip, or even a surf retreat to maximize your stay. As locals of Essaouira, we know the best spots to take you, regardless of your skill level. We offer surf lessons and surf trips for all abilities, from beginners to advanced surfers looking to enhance their technique. Our surf lessons are tailored to your needs, ensuring you get the most out of your surf holiday.",
			"We are passionate surfers who embrace the beach lifestyle. Our goal is to ignite that same love for the ocean within you. From sunrise to sunset, we provide an opportunity to connect with nature, ride the waves, and immerse yourself in the local culture. Each surf spot in Morocco has its unique charm waiting to be explored. Experience the joy of surfing in Morocco with us and discover the beauty of this incredible destination.",
			"Join the Surftwins Essaouira for an unforgettable surf adventure!"]

		},
		{
		img: 'https://cdn.prod.website-files.com/617b6f00715044249cb2b8dc/660aa6ed85ab65ca8c858bda_kite%20surftwins%20wave%20.JPG',
		name: 'Experience the thrill of kitesurf in essaouira morocco',
		paragraphs: [
			"Welcome to Essaouira, a renowned destination for kitesurf and kiteboarding enthusiasts. The Surftwins Essaouira offers kitesurf exciting lessons led by experienced instructors, catering to all levels and abilities.",
			"The bay in Essaouira provides a safe and sheltered environment with side-on winds, perfect for learning and progression. Beginners can use flat water spots during high tide to practice water starts. At the same time, more experienced kitesurfers can enjoy the mix of choppy water and kitesurfing waves to enhance their skills.",
			"When not on the water, explore the vibrant old Medina for a diverse and memorable holiday experience. Join the Surftwins Essaouira for an exhilarating kitesurf adventure!"]


		},
		{
		img: 'https://cdn.prod.website-files.com/617b6f00715044249cb2b8dc/660aa8fe2440c8679f072bd0_surftwins%20essaouira%20on%20trip%20.JPG',
		name: 'Additional Experiences to Enhance Your Moroccan Vacation in essaouira',
		paragraphs: [
		"Morocco offers a wide range of experiences beyond surfing. Make the most of your Moroccan holiday with activities in Essaouira like sightseeing, camel riding, quad biking, and horseback riding. Explore the vibrant Moroccan souks, hike to stunning waterfalls, or learn to cook traditional Moroccan dishes.",
		"At the Surftwins Essaouira, we want you to have an unforgettable Moroccan holiday. Indulge in our favorite local restaurants, relax in Hamams, or enjoy beachside barbecues as the sun sets. With endless activities to fill your holidays, we're excited to welcome you and show you a great time in Morocco."
		]
		}
	];

	const paragraphs = [];
</script>


<Hero></Hero>

<div class="page-wrapper">
	<div class="section">
		<div class="pattern"></div>
		<div>
			<img
				src="https://cdn.prod.website-files.com/617b6f00715044249cb2b8dc/617b76d98653f3ca6e28afd7_enjoy-morroc-surftwins.svg"
				loading="lazy"
				alt="chill-morroc"
				class="intro-img"
			/>
			<div class="intro-text">
				Surf, Eat, drink &amp; Chill
				<br />
				enjoy an endless Moroccan summer with
				<br />
				the Surftwins essaouira
			</div>
		</div>
	</div>
</div>

<Offers></Offers>

<!-- <div class="section">
	<h2>Why choose to surf or kitesurf with us?</h2>
	<div class = "cards-wrapper">
		<div class = "card">
				<img src="https://cdn.prod.website-files.com/617b6f00715044249cb2b8dc/617b79960ca40d1bc6ad6923_brandshaper-icon-fun.svg"/>
				<p>poo</p>
				<div class = "separator"> </div>
				<p>Increase your happiness hormones with enjoyable activities that boost endorphins!</p>
		</div>
		<div class = "card">
				<img src="https://cdn.prod.website-files.com/617b6f00715044249cb2b8dc/617b79960ca40d1bc6ad6923_brandshaper-icon-fun.svg"/>
				<p>pee</p>
				<div class = "separator"> </div>
				<p>We offer exclusive private group sessions for enhanced collaboration and learning.</p>
		</div>
		<div class = "card">
				<img src="https://cdn.prod.website-files.com/617b6f00715044249cb2b8dc/617b79960ca40d1bc6ad6923_brandshaper-icon-fun.svg"/>
				<p>shit</p>
				<div class = "separator"> </div>
				<p>No need to worry about dangerous currents or sharp rocks. We carefully select safe spots for your peace of mind.</p>
		</div>
		<div class = "card">
				<img src="https://cdn.prod.website-files.com/617b6f00715044249cb2b8dc/617b79960ca40d1bc6ad6923_brandshaper-icon-fun.svg" />
				<p>frick</p>
				<div class = "separator"> </div>
				<p>Relax and enjoy a great time with like-minded individuals who crave adventure.</p>
		</div>
	</div>
</div> -->

<!-- <Carousel></Carousel> -->

 <section id = "columns">
	{#each columns as col, i}
		<Column {...col}>
		</Column>
	{/each}
 </section>

 
<div class = "column">

</div>


<style lang="scss">
	
	// (750 x 1334 pixels) 

	@import url('https://fonts.googleapis.com/css2?family=Nunito:wght@200..1000&family=Red+Hat+Display:ital,wght@0,300..900;1,300..900&display=swap');
	* {
		font-family: 'Red Hat Display', sans-serif;
		color: white;
		text-decoration: none;
	}

	.column {
		display: grid;
		grid-template-columns: 1fr;

		grid-column-gap: 32px;
		grid-row-gap: 32px;
		border: 2px solid red;
		// height: auto; this is default i think ..
		position: relative;

		place-items: center stretch;
		width: 100vw;

		// min-height: 65vh;
		// margin-top: 60px;
		// margin-bottom: 60px;
		overflow: hidden;
		// box-sizing: border-box; // this fixed div being wider than viewport but not part of reference code
	}

	@media screen and (max-width: 400px) {
		.column {
			grid-template-columns: 1fr;
			background-color: rgba(255,0,0,.25);
		}
	}


	.section {
		text-align: center;
		object-fit: fill;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		width: 100vw;
		//padding: 60px; revert?

		box-sizing: border-box;

		//padding-right: 00px;
		display: block;
		position: relative;
	}

	

	p {
		border-left:  2px solid white;

	}


	@media screen and (max-width: 400px) {

	.column {
		grid-template-columns: 1fr;
		background-color: rgba(255,0,0,.25);

	}
}
    
	@media screen and (min-width:475px){ 

	
	.column {
		display: grid;
		// grid-template-rows: auto; // why??
		grid-template-columns: 1fr 1fr;
		//grid-auto-columns: 1fr; // why ??
		grid-column-gap: 32px;
		grid-row-gap: 32px;
		border: 2px solid red;
		// height: auto; this is default i think ..
		position: relative;
		//align-items: center;
		place-items: center stretch;
		width: 100vw;
		// padding: 60px;
		min-height: 65vh;
		// margin-top: 60px;
		// margin-bottom: 60px;
		overflow: hidden;
		box-sizing: border-box; // this fixed div being wider than viewport but not part of reference code
		
	}

	@media screen and (max-width: 400px) {
		.column {
			grid-template-columns: 1fr;
			background-color: rgba(255,0,0,.25);

		}

	}


	.section {
		text-align: center;
		object-fit: fill;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		width: 100vw;
		padding: 60px;

		box-sizing: border-box;


		display: block;
		position: relative;
	}



	p {
		border-left:  2px solid white;
	}



	}



	




</style>
