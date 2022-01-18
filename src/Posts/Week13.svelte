<script>
    import Post from "../Post.svelte";
    import Title from "../Title.svelte";
    import Text from "../Text.svelte";
    import Image from "../Image.svelte";
</script>

<Post>
    <Title>XR Project Week 4 "Rampage"</Title>
    <Text>
        <a href="https://youtu.be/Mum_q_5U_lY">Link to Video</a>
    </Text>
    <Text>
        <p>
            As the main components were set, it was time to focus on polishing
            the game for the VR/XR expo.
        </p>
        <p>
            In order to make the final game more enjoyable the team decided on implementing the following
             functionality:
        </p>
        <ol>
            <li>
                Adding a user interface to provide feedback to the player.
            </li>
            <li>
                Allowing the user to select between two levels, the first one for getting the feel of the game and its 
                environment, while the second one being more of a challenge as enemies rise from the floor and chase
                after the player.
                <Image src="level1.png"/>
                <Image src="level2.png"/>
            </li>
            <li>
                Including sounds in the game to make the whole experience more imersive.
            </li>
            <li>
                Included textures in the environment in order to make the game more visually appealing.
            </li>
        </ol>

        <p>
            The last thing that was worked on was tweaking some aspects of features such as:
        </p>
        <ol>
            <li>
                Grapple pulling speed
            </li>
            <li>
                Monster spawn speed
            </li>
            <li>
                Death when interacting with the mobs as well as the lava
            </li>
        </ol>
    </Text>
</Post>
