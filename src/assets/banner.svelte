<script>
    // import Youtube from "svelte-youtube-embed";
    // import Youtube from "./Youtube.svelte";

    // Data
    import {banner_data} from "../data.ts";

</script>


<!------------------------------------------->
<!----------------MARKUP----------------------->
<!------------------------------------------->
<section class="main-bgcolor light-color" id="banner">
    <div class="container">
        <div class="row">
            <div class="col-md-6">
                <h1>{banner_data.HEADING}</h1>
                <p>{banner_data.DESCRIPTON_SHORT}</p>
                <a href={banner_data.VIDEO_URL} target=”_blank” class=”light-color”>
                    <i class="fa fa-play-circle fa-2x watch-btn"></i>KIJk ONZE TRAILER
                </a>
            </div>
            <div class="col-md-6">
<!--                <Youtube id={banner_data.VIDEO_ID}/>-->
                <img src="groepsfoto3.jpg" alt="" class="group-pic" />
            </div>
        </div>
    </div>
    <img src="wave1.png" alt="hello" class="banner-img"/>
</section>


<!------------------------------------------->
<!----------------STYLE----------------------->
<!------------------------------------------->
<style>
    section {
        padding-top: 2.5%;
    }
    h1 {
         font-size: 40px;
         font-weight: 600;
         margin-top: 100px;
         text-transform: uppercase;
     }

    .watch-btn {
        margin: auto 20px;
        position: relative;
        top: 8px;
        color: var(--subsub-green);
    }

    .banner-img {
        width: 100%;
        height: auto;
        display: block;
    }
    .group-pic {
        width: auto;
        height: 425px;
        padding: 0;
        display: block;
    }

    section a {
        text-decoration: none;
    }
</style>