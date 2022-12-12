<script>

    import {service_data} from "../data.ts";


</script>

<section id="services" class="section">
    <div class="container text-center">
        <img src="/logo_transparant.png" class="logo" alt="Bende logo" />
<!--        <h2 class="title">{service_data.HEADING}</h2>-->
        <div class="row section-body">
            {#each service_data.SERVICE_LIST as list}
                <div class="col-md-4 service">
<!--                    <img src={list.URL} alt={list.LABEL} class="service-img" />-->
                    <h4>{list.LABEL}</h4>
                    <p>{list.DESCRIPTION}</p>
                </div>
            {/each}
        </div>
<!--        <buttom class=”btn btn-primary round-border main-bgcolor”>-->
<!--            {ALL_SERVICES}-->
<!--        </buttom>-->
    </div>
</section>


<style>
    .logo {
        height: 6em;
        padding: 0em;
        will-change: filter;
    }
    .service-img {
        width: 200px;
        height: 200px;
        margin-top: 20px;
    }
    .service h4 {
        padding: 5px;
        margin-top: 25px;
        font-size: x-large;
        /*text-transform: uppercase;*/
    }
    .title {
        text-transform: uppercase;
        font-size: xx-large;
        color: #1a1a1a;
    }
    .title::before {
        content: "";
        background: var(--gradient);
        height: 5px;
        width: 200px;
        margin-left: auto;
        margin-right: auto;
        display: block;
        transform: translateY(60px);
    }
    /*.title::after {*/
    /*    content: "";*/
    /*    background: var(--gradient);*/
    /*    height: 10px;*/
    /*    width: 50px;*/
    /*    margin-left: auto;*/
    /*    margin-right: auto;*/
    /*    margin-bottom: 40px;*/
    /*    display: block;*/
    /*    transform: translateY(14px);*/
    /*}*/
    section .btn-primary {
        box-shadow: none;
        padding: 8px 25px;
        border: none;
    }
</style>