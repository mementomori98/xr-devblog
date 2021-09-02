<script>

</script>

<div class="post">
    <slot/>
</div>

<style lang="scss">
    @import "globals.scss";

    .post {
        padding: 32px;
        border: 1px solid #d3d3d3;
        background-color: #fcfcfc;
        border-radius: 8px;
        line-height: 1.5em;
        margin-bottom: 40px;
    }

    :global(.post * + *) {
        margin-top: 24px;
    }
</style>