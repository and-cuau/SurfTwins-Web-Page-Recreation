<section class="hero-homepage">
	<div class="container">
		<h1 class="home-h1">Learn to surf the fun way with the SurfTwins</h1>
		<p class="subhead">
			Experience the thrill of riding local Moroccan waves while guided by highly skilled
			instructors who uphold exceptional teaching standards.
		</p>
		<a href="/en/contact" class="button w-button">DM us for booking</a>
	</div>

    <div class = "ta-div">
        <img class = "ta-logo" src = "https://www.freepnglogos.com/uploads/tripadvisor-logo-png/tripadvisor-logo-tripadvisor-logotype-social-icons-11.png">
        <img class = "stars" src = "https://www.pngmart.com/files/10/5-Stars-PNG-Isolated-HD.png">
        <p class = "enjoy"> Over 400 customers enjoyed lessons with our qualified instructors on the Morrocan coast</p>
    </div>
</section>


<div data-w-id="2b9fc718-4ab8-3ff6-53e4-eee1e355b5a9" class="menu-button">
    <div class = "line"></div>
    <div class = "line"></div>
    <div class = "line"></div>
</div>


<meta name="viewport" content="width=device-width, initial-scale=1">

<style lang="scss">
    @import url('https://fonts.googleapis.com/css2?family=Nunito:wght@200..1000&family=Red+Hat+Display:ital,wght@0,300..900;1,300..900&display=swap');
	* {
	font-family: 'Red Hat Display', sans-serif;
	}

	section {
		background-image:
			linear-gradient(#fdfcfc00 67%, #fdfcfc99 94%), linear-gradient(96deg, #21212133 22%, #0000),
			url(https://cdn.prod.website-files.com/617b6f00715044249cb2b8dc/617fac6dca16ae36a22a0c29_about_header.jpg);
		height: 100vh;
		// background-position:
		// 	0 0,
		// 	0 0,
		// 	50% 0;  //
            overflow: hidden;
            background-size: cover;
            background-position: right center;
	}

	.container {
		//max-width: 850px;
		margin: 80px 0; // top right bottom left
	}

	h1 {
		max-width: 500px;
        width: auto;
		font-size: 8vw;
		text-wrap: balance;
		text-transform: uppercase;
        margin: 0px auto;
        text-align: center;
    }

	.subhead {
		// max-width: 400px;
		text-align: center;
		margin: 50px 0 0 0;
        display: none;
	}

	.button.w-button {
		padding: 12px 32px;
		background-color: rgb(232,131,43);
		border-radius: 100px;
		text-decoration: none;
		color: white;
        width: fit-content;
        margin: 20px auto;
        display: block; //needs to be disp. block (or in-line block?) for margin auto to work
        text-align: center;
	}

	section.hero-homepage {
		color: #fdfcfc;
		text-align: left;
		background-image:
			linear-gradient(#fdfcfc00 67%, #fdfcfc99 94%), linear-gradient(96deg, #21212133 22%, #0000),
			url(https://cdn.prod.website-files.com/617b6f00715044249cb2b8dc/617fac6dca16ae36a22a0c29_about_header.jpg);
		background-position:
			0 0,
			0 0,
			50% 0;
		background-size: auto, auto, cover;
		height: 100vh;
        width: 100vw;
		//min-height: 700px;
		display: block;
        background-position: 79% 40%;
		position: relative;
	}

    .ta-logo{
       // margin: 0px auto;
        height: 40px;
        width: 35px;
    }

    .ta-div{
        height: 100px;
        width: 80px;
        display: flex;
        flex-direction: column;
        margin: 250px 0 0 0;
        height: 150px;
        width: 100%;
        // border: 2px solid red;
        // flex-wrap: wrap;
        align-items: center;
    }

    .stars{
        height: 20px;
        width: 100px;
      
    }

    .enjoy{
        text-align: center;
    }
   @media screen and (min-width: 376px) {
        // h1{
        //     font-size: 10vw;
        //   }

         section.hero-homepage{
             background-position: 79% 40%;
             height: 100vh;
         }

		h1{
			font-size: 3vw;
			font-weight: bold;
			text-align:left;
			margin: 30px 0;
		}

		.container{
			margin-right: 60px;
			margin-left: 60px;
		}

		.button.w-button{
			margin: 30px 0;
		}


		.ta-div{
			margin-top: 470px;
		}

    }

</style>
