<script>
    import { Footer, Button, MaterialApp } from 'svelte-materialify';

    const items = ['Home', 'About', 'Our music']

</script>

<MaterialApp>
    <Footer padless class="green theme--dark justify-center flex-column">
        <div class="mt-2 mb-2">
            {#each items as item}
                <Button text rounded>{item}</Button>
            {/each}
        </div>
        <div class="green lighten-1 pa-2 text-center" style="width:100%">
            2022 -
            <b>De Bende</b>
        </div>
    </Footer>
</MaterialApp>