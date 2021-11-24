<script>
    import Post from "../Post.svelte";
    import Title from "../Title.svelte";
    import Text from "../Text.svelte";
</script>

<Post>
    <Title>VR Week 2 - Minecraft VR</Title>
    <Text>
        During this week we decided on the specifics of our "Minecraft VR" game.

        We decided on the following based on the time left and complexity of the task.
    </Text>
        <ol>
            <li>The game would only allow you to create and destroy objects.</li>
            <li>The player would have a set of different materials to choose from such as: 
                <ol>
                    <li>
                        A dirt block
                    </li>
                    <li>
                        A grass block
                    </li>
                    <li>
                        A diamond block
                    </li>
                    <li>
                        A stone block
                    </li>
                 </ol>
            </li>
        </ol>
        <Text>
            The primary challenges that the team had to solve were two:
        </Text>
        <ol>
            <li>How do you make cubes perfectly "snap to eachother"?</li>
            <li>How do you keep track of your controller postion in the VR world smooth and not in the way?</li>
        </ol>
    <Text>
        The team came up with the following solutions.
        <ol>
            <li><Text>In order to make the cubes "snap to eachother", the team decided to use a raycast which does the following. Upon pressing the trigger
            on the controller, a raycast is fired to a cube. The information from the raycast hit is therefore used to identify the side
            of the cube the player is trying to attach the new cube on. The perpendicular, normalized Vector of that side is therefore retrieved to identify in which direction the new 
            cube is to be placed. The cube is then placed exactly 0.5 meters away from the other cube due to the fact that the surfice area of each side is exactly 1m2.

            </Text>
            </li>
            <li>
                <Text>
                    In order to display where the player is pointing at exactly, the team decided to try out two options.
                    <ol>
                        <li>
                            Firstly, a lazer was drawn from the position of the controller in the direction in which it is pointing at. Although
                            a simple solution, it proved not to be as useful. The problem was that the player was able to see the direction where he was pointing at, but no the exact position.
                            That resulted in the player misplacing cubes which is far away from ideal.
                        </li>
                        <li>Upon examination of the first method, the team decided to implement a "sticky tracker". Another raycast was used to implement this function.
                            In essence, the feature works by spawing a circle wherever the continiously fired raycast hits. That allowed for a perfect level of precision when placing or destroying blocks
                        </li>
                    </ol>
                </Text>
            </li>
        </ol>
    </Text>
    <p>Check out a video of our game <a href="https://youtu.be/9fe1RBhZlwk"
    >here! </a>
    </p>
</Post>