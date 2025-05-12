<script>

    let index = 1;

    let images = ["image1.jpg", "image2.jpg", "image3.jpg"];


    function prev() {
        index = (index + 1) % images.length;
    }
    function next() {
        index = (index - 1 + images.length) % length; 
    }


</script>


<div class = carousel>
	<h2>You are in good company with the Surftwins Essaouira</h2>
	<h2>But don’t just take our word for it</h2>

    <img src = "https://cdn.prod.website-files.com/617b6f00715044249cb2b8dc/617b7fb5a51183340f0c1ec7_testimonial_1.jpg">
    <img src = "https://cdn.prod.website-files.com/617b6f00715044249cb2b8dc/617b7fb5a511837c4d0c1ecd_testimonial_2.jpg">
    <img src = "https://cdn.prod.website-files.com/617b6f00715044249cb2b8dc/617b7fb5a511833ea80c1ec5_testimonial_3.jpg">

</div>


<style lang="scss">
.carousel{

    

    img{
       width: 100%;
       height: auto;
    }
}



</style>


