<script>
    import Post from "./Post.svelte";
    import Title from "./Title.svelte";
    import Code from "./Code.svelte";
    import Tab from "./Tab.svelte";
    import Image from "./Image.svelte";
    import Text from "./Text.svelte";
    import Nfsw from "./Nfsw.svelte";
    import Week1 from "./Posts/Week1.svelte";
    import Week2 from "./Posts/Week2.svelte";
    import Week6 from "./Posts/Week6.svelte";
    import Week5 from "./Posts/Week5.svelte";
    import Week4 from "./Posts/Week4.svelte";
    import Week3 from "./Posts/Week3.svelte";
    import Week7 from "./Posts/Week7.svelte";
    import Week8 from "./Posts/Week8.svelte";
    import Week9 from "./Posts/Week9.svelte";
    import Week10 from "./Posts/Week10.svelte";
    import Week11 from "./Posts/Week11.svelte";
    import Week12 from "./Posts/Week12.svelte";
    import Week13 from "./Posts/Week13.svelte";

    var order = false;

</script>

<div class="layout">
    <div class="appbar">
        <div class="button" on:click={() => order = false}>Oldest First</div>
        <div class="button" on:click={() => order = true}>Newest First</div>
    </div>
    <div class="content">
        {#if order}
            <Week13/>
            <Week12/>
            <Week11/>
            <Week10/>
            <Week9/>
            <Week8/>
            <Week7/>
            <Week6/>
            <Week5/>
            <Week4/>
            <Week3/>
            <Week2/>
            <Week1/>
            {:else }
            <Week1/>
            <Week2/>
            <Week3/>
            <Week4/>
            <Week5/>
            <Week6/>
            <Week7/>
            <Week8/>
            <Week9/>
            <Week10/>
            <Week11/>
            <Week12/>
            <Week13/>
            {/if}

    </div>
</div>

<style lang="scss">
    @import "globals.scss";

    .button {
        padding: 8px 16px;
        color: white;
        border-radius: 6px;
        cursor: pointer;
        user-select: none;
    }

    .button:hover {
        background-color: rgba(255, 255, 255, 0.1);
    }

    :global(body) {
        margin: 0;
    }

    :global(*) {
        font-family: sans-serif;
        font-size: 20px;
        box-sizing: border-box;
    }

    .layout {
        display: flex;
        flex-direction: column;
        align-items: center;
        background-color: #f8f8f8;
        min-height: 100vh;
    }

    .appbar {
        height: 48px;
        box-shadow: 0 0 5px 1px rgba(0, 0, 0, 0.5);
        width: 100%;
        background-color: #207796;
        z-index: 10;
        position: fixed;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .content {
        max-width: 900px;
        width: 100%;
        flex: 1;
        background-color: white;
        padding: 40px;
        box-shadow: 0 0 4px 1px rgba(0, 0, 0, 0.3);
        margin-top: 48px;
    }
</style>