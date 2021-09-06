<script>
    import Post from "./Post.svelte";
    import Title from "./Title.svelte";
    import Code from "./Code.svelte";
    import Tab from "./Tab.svelte";
    import Image from "./Image.svelte";
    import Text from "./Text.svelte";
    import Nfsw from "./Nfsw.svelte";
</script>

<div class="layout">
    <div class="appbar">

    </div>
    <div class="content">
        <Post>
            <Title>Day 1 in lab</Title>
            <Text>Our heroes went to the XR lab to live up to their intelligence and creativity, testing out the endless possibilities with Augmenting reality to match their desires.</Text>
            <Text>Time was spent downloading and experimenting with the AR Camera and ImageTarget objects of Vuforia, getting familiar with the framework (also Unity) and experimenting with configurations.</Text>
            <Nfsw>
                <Image src="https://scontent.xx.fbcdn.net/v/t1.15752-9/241359609_710846843218162_2915078542196166342_n.jpg?_nc_cat=103&ccb=1-5&_nc_sid=aee45a&_nc_ohc=5B_4KdDd-LsAX8nC-pU&_nc_ad=z-m&_nc_cid=0&_nc_ht=scontent.xx&oh=38263e453374b4394d25e29d2526b753&oe=615D109A"/>
            </Nfsw>
        </Post>
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