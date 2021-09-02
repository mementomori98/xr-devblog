<script>
    export let src;
</script>

<div class="image">
    <img src={src}/>
</div>

<style lang="scss">
    .image {
        display: flex;
        justify-content: center;
        padding: 16px 0;

        :global(& img) {
            width: 80%;
            display: block;
            border-radius: 10px;
            box-shadow: 0 0 3px 1px rgba(0, 0, 0, .5);
        }
    }
</style>