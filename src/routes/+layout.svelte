<script lang="ts">
	let { children } = $props();
	import './global.scss';
</script>


<!-- <img src="https://cdn.prod.website-files.com/617b6f00715044249cb2b8dc/65f2cc6698582651c7c2f0e9_SURF_TWINS_LOGO_ORANGE%20edit.png" loading="lazy" width="Auto" height="Auto" alt="" srcset="https://cdn.prod.website-files.com/617b6f00715044249cb2b8dc/65f2cc6698582651c7c2f0e9_SURF_TWINS_LOGO_ORANGE%20edit-p-500.png 500w, https://cdn.prod.website-files.com/617b6f00715044249cb2b8dc/65f2cc6698582651c7c2f0e9_SURF_TWINS_LOGO_ORANGE%20edit.png 806w" sizes="(max-width: 991px) 100px, 140px" class="logo-navbar"> -->

<nav>
	<a href="/">
		<img src="https://cdn.prod.website-files.com/617b6f00715044249cb2b8dc/65f2cc6698582651c7c2f0e9_SURF_TWINS_LOGO_ORANGE%20edit.png" loading="lazy" width="Auto" height="Auto" alt="" srcset="https://cdn.prod.website-files.com/617b6f00715044249cb2b8dc/65f2cc6698582651c7c2f0e9_SURF_TWINS_LOGO_ORANGE%20edit-p-500.png 500w, https://cdn.prod.website-files.com/617b6f00715044249cb2b8dc/65f2cc6698582651c7c2f0e9_SURF_TWINS_LOGO_ORANGE%20edit.png 806w" sizes="(max-width: 991px) 100px, 140px" class="logo-navbar"> 
	</a> 

	<div class = "container">
		<a href="/about">About</a>
		<a href="/blog">Blog</a>
		<a href="/">offer</a>
		<a href="/booking" id = "test">book now</a>
	</div>

	<div id = "menubutton">
		<div class = "line"></div>
		<div class = "line"></div>
		<div class = "line"></div>
	</div>

</nav>

{@render children()}



<style lang="scss">


	@import url('https://fonts.googleapis.com/css2?family=Nunito:wght@200..1000&family=Red+Hat+Display:ital,wght@0,300..900;1,300..900&display=swap');

	* {
	font-family: 'Red Hat Display', sans-serif;
	}


	a {
			font-size: 16px;
			text-decoration: none;
			color: #fdfcfc;
			//padding: 0 20px;
			text-transform: uppercase;
		}

		#test{
			background-color: #ad5b13;
			border-radius: 100px;
			
		}

		img{
			height: 100%;
			width: auto;
			//  justify-self: flex-start;


			align-self: center;
		}
		
		.line {
			// border: 2px solid red;
			display:flex;
			align-items: center;  // only for flex and grid containers. vertical axis
			z-index: 100;
			background-color: black;
			height: 2px;
			width: 25px;
		}

		nav {
			//justify-content: flex-end; // main axis (horizontal by default)
			display: flex;
			// padding: 0 60px;
			box-sizing: border-box;
			height: 10vh;
			width: 100%;
			z-index: 1000; //?
			background-image: linear-gradient(#2e2e2e80,#0000);
			// gap: 0vw;
			position: absolute;
			box-sizing: border-box;	
			padding: 0 20px;
		}

		#menubutton{
			display: flex;
			flex-direction: column;
			align-self: center;
			//justify-self: flex-end; justify self not used for flex children
			margin-left: 50vw; // surf site does this diferently no left margin idk how
			//margin-right3: 20px;
			// grid-template-columns: 1fr;
			 row-gap: 4px;
		}

		.line{
			background-color: white;
			height:2px;
		
		}

		.container{
			display:none;
		}



	@media screen and (min-width: 376px){
		a {
			font-size: 16px;
			text-decoration: none;
			color: #fdfcfc;
			padding: 0 20px;
			text-transform: uppercase;
		}

		#test{
			background-color: #ad5b13;
			border-radius: 100px;
		}

		img{
			height: auto;
			width: auto;
			//justify-self: flex-start;
			position: relative;
			align-self: center;
		}
		
		div {
			// border: 2px solid red;
			//display:none;
			align-items: center;  // only for flex and grid containers. vertical axis
			z-index: 100;
		}

		nav {
			 justify-content: space-between;
			display: flex;
			padding: 0 90px;
			height: 100px;
			width: 100%;
			z-index: 1000; //?
			background-image: linear-gradient(#2e2e2e80,#0000);
			// gap: 40vw;
			position: absolute;
		}

		#menubutton {
			display: none;
		}

		.container{               // No, justify-self will not work in a flex container because justify-self is only applicable to grid layouts, not flexbox.
			//justify-self: flex-end;
			display: block;
			position: relative;
		}

	}

</style>  