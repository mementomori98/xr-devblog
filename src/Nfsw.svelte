<script>
    let show = false;
</script>

<div class="nsfw">
    {#if show}
        <div on:click={() => show = !show} >
            <slot />
        </div>
        {:else }
        <div class="nsfw__disclaimer"  on:click={() => show = !show}>
            <div class="nsfw__disclaimer-title">
                NSFW
            </div>
            <div class="nsfw__disclaimer-content">
                [ Click to View anyways ]
            </div>
        </div>
    {/if}
</div>

<style lang="scss">
    @import "globals.scss";

    .nsfw__disclaimer {
        box-shadow: $shadow;
        padding: 32px;
        text-align: center;
        user-select: none;
        border-radius: 4px;
    }

    .nsfw {
        cursor: pointer;
    }

    .nsfw__disclaimer-title {
        font-size: 32px;
        font-weight: bold;
    }
</style>