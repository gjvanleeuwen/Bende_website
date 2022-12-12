<script>
    import {navbar_items} from "../data.ts";
</script>


<section id="nav-bar">
    <nav class="navbar navbar-expand navbar-light main-bgcolor">
        <a class="navbar-brand light-color" href="/">
            De Bende
        </a>
        <button class="navbar-toggler" type="button" data-toggle="collapse"
                data-target="#navbarNav" aria-controls="navbarNav"
                aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse justify-content-end light-color" id="navbarNav">
            <div class="navbar-nav light-color">
                <!--{navbar_items}-->
                {#each navbar_items as item}
                    <a class="nav-item nav-link light-color" href={item.url}>{item.label} </a>
                {/each}
            </div>
        </div>
    </nav>
</section>


<style>
    #nav-bar {
        position: sticky;
        top: 0;
        z-index: 10;
    }
    .navbar {
        padding: 0 20px !important;
    }
    .navbar-nav {
        font-weight: 600;
        text-transform: uppercase;
        float: right;
        text-align: left;
    }
</style>