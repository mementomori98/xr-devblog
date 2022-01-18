<script>
    import Post from "../Post.svelte";
    import Title from "../Title.svelte";
    import Text from "../Text.svelte";
</script>

<Post>
    <Title>AR Marker based week 2 - Finishing the Paddle Game</Title>
    <Text>
        <a href="https://youtu.be/_wUkYXnn2nM">Link to Video</a>
    </Text>
    <Text>
        In the second week of the marker based VR project we managed to finish up our Paddle game project.
    </Text>
    <Text>
        As we had a preset map for the game, we decided that we do not want to have just a bunch of prefabs copied around the playing area, as it
        would be a bad design choice for future game improvements like adding more levels. We implemented this by generating the prefabs and setting the bounds so they wouldn't
        be outside the play space
    </Text>
    <Text>
        We also implemented a win and lose screen if the player manages to either hit all the blocks and win or miss the ball with the paddle and lose. This was made with a counter
        for the block which reaches a certain count and triggers the win game screen or if you miss the ball and it goes out of bound of the play area, it triggers the lose screen
        and restarts the game.
    </Text>
</Post>
