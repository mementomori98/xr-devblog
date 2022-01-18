<script>
    export let src;
</script>

<div class="image">
    <img src={src} style=""/>
</div>

<style lang="scss">
    @import "globals.scss";
    .image {
        display: flex;
        justify-content: center;
        padding: 16px 0;

        :global(& img) {
            max-height: 500px;
            max-width: 100%;
            display: block;
            border-radius: 10px;
            box-shadow: $shadow;
        }
    }
</style>