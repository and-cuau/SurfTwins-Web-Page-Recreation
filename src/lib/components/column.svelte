<script lang="ts">
     const {img, name, paragraphs } = $props();
</script>


<div class = "column">
    <img src = {img}>

    <div class = "container">
        <div class = "text-wrap">
            <h3>{name}</h3>
            {#each paragraphs as p}
                <p>{p}</p>
            {/each}
        </div>
    </div>

   
</div>

<style lang="scss"> 

    .column{
        display: grid;
        grid-template-rows: auto auto;
		border: 2px solid red;
        
        height: auto;
        width: 100vw;

    }

    .column img{
        width:100%;

    }

    h3{
        text-transform: uppercase;
    }

@media screen and (min-width: 476px){

    .column{
         grid-template-columns: 1fr 1fr;
         grid-template-rows: 1fr;
    }

    .column img{
        width:100%;
        height: auto;
    }


    .container{
        position: relative;
    }

    .text-wrap{
       // height: 100%;
        width: 300px;
        position: relative;
        margin-left: 100px;
    }

}




</style>