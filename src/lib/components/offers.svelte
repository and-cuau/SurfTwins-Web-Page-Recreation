
<script>
    const offers = [
		{
			title: 'Day Surf Trip',
			sub: 'Starting from 50€',
			href: '/',
			src: 'https://cdn.prod.website-files.com/617b6f00715044249cb2b8dc/67af4c04993963c923fb8a13_IMG_4215.jpg'
		},
		{
			title: 'Kite Surf Lessons',
			sub: 'Starting from 60€',
			href: '/',
			src: 'https://cdn.prod.website-files.com/617b6f00715044249cb2b8dc/6341f4b1be51d063cd0288b2_IMG-4547.jpg'
		},
		{
			title: 'Surf Lesson',
			sub: 'Starting from 30€',
			href: '/',
			src: 'https://cdn.prod.website-files.com/617b6f00715044249cb2b8dc/6644f943d9f3d420bc3f3e75_surftwins%20surfing%20.jpg'
		},
		{
			title: 'Surf Camp - In No Ordinary Way',
			sub: 'Starting from 380€',
			href: '/',
			src: 'https://cdn.prod.website-files.com/617b6f00715044249cb2b8dc/66febc357e94f0461149becd_surf%20lesson%20in%20sidi%20kaouki.jpeg'
		}
	];
</script>



<section id = "offers">
	<div class = "header">
		<p>Can't wait any longer?</p>
		<h2>Discover your perfect surf or kitesurf adventure today</h2>
	</div>
	<div class = "offers-container">
		{#each offers as offer}
				<a class="offer" href={offer.href}>
					<img src = {offer.src} alt = "" />
					<div class = "content">
						<h3>{offer.title}</h3>
						<p>{offer.sub}</p>
					</div>
				</a>
		{/each}
	</div>
</section>



<style lang="scss">
  #offers{
  //  margin: 60px 0;

     .header{
         p{
             text-align: center;
         }
         h2{
             text-align: center;
         }
     }

     .offers-container{
             display: grid;
             grid-template-columns: 1 fr;
             grid-template-rows: repeat(4, 1fr);
             gap: 20px;
             padding: 0 32px;

              .offer{
                  // padding: 0 30px;
                  box-sizing: border-box;
                  position: relative;
                   //height: auto;
                   contain: paint;
                  width: 100%;
                 &:hover {
                         transform: scale(1.01) translateY(-10px);
                 }
                 .content{
                    position:absolute;
                    // left: 32px;
                       bottom: 32px;
                       color:white;
                    h3{
                        font-size: 25px;
                        margin: 0;
                    }
                    p{
                        font-size: 10px;
                        margin:0px;
                    }
                 }
             }
     }
      img{
        object-fit: cover;
          width: 100%;
          height: 100%;
      }
   }

   @media screen and (min-width: 376px){
    #offers{


        .offers-container{
            grid-template-columns: 1fr 1fr;
            grid-template-rows: repeat(2, 1fr);
        }


    }

   }

</style>