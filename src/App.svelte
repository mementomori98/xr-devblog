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
</script>

<div class="layout">
    <div class="appbar">

    </div>
    <div class="content">
        <Week2/>
        <Week1/>
    </div>
</div>

<style lang="scss">
    @import "globals.scss";

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