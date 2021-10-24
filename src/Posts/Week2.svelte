<script>
    import Text from "../Text.svelte";
    import Title from "../Title.svelte";
    import Post from "../Post.svelte";
    import Image from "../Image.svelte";
</script>

<Post>
    <Title>AR Marker based Week 1 - Foundations of an AR Game</Title>
    <Text>
        This week we outlined our plan for our app. A game where you control a pad to prevent a ball from falling,
        which then bounces back up to break bricks and score points for the player.
        We laid out the skeleton.
    </Text>
    <Text>
        Some problems we had to solve were the following:
    </Text>
    <Text>
        Firstly, we needed to have a stable foundation for the world, which was our first image target.
        The image target was a reference to an empty GameObject, which was our "World". Everything that belonged
        to our world, except for the Pad should be a child object to this one.
    </Text>
    <Text>
        Secondly, we needed to solve the issue of having multiple image targets, and having their coordinates corresponding to each other
        without having really awkward spacing. The images will be laid out in 3D space, while the game is 2D-like, and the pad should
        only move in 1 dimension.
        To solve the problem, the pad had 2 coordinates locked (Y and Z), while the X coordinate was given by the X coordinate
        of the detected image target. Below picture shows that PadOrigin (the image target) only passes it's X coordinate to the Pad (gameObject).
    </Text>
    <Image src="code1.png"/>
    <Text>This way the player can have their image positioned anywhere in real space, giving a smooth experience.</Text>
    <Text>
        Thirdly, the ball collision and velocity had to be implemented. Same as for the pad, the ball had its Y coordinate locked, because
        some of the colliders gave a slight movement towards the Y axis, which resulted in the ball flying out of game space.
        The velocity of the ball was always a normalized direction vector multiplied by a constant, therefore always moving at the same speed.
    </Text>
    <Image src="pic1.png"/>
</Post>