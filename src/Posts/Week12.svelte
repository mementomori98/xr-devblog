<script>
    import Post from "../Post.svelte";
    import Title from "../Title.svelte";
    import Text from "../Text.svelte";
    import Image from "../Image.svelte";
</script>

<Post>
    <Title>XR Project Week 3 "Annihilation"</Title>
   <Text><p>Since we already had the main mechanic in place, we decided it's time to break it up a little.</p>
        <p>The next thing on the list was the enemies. Since the team was was "The floor is lava", we decided to go
            with a nice fire monster pack for the enemies.</p>
            <Image src="FireMonster.png"/>
            <p>Having the model for the enemies, it was time to make them evil! Therefore we created the EnemeyAI script
                which was in charge of giving them a stalker like nature. Wherever you go, whatever you do, their eyes are locked at you and they are going for the kill!
            </p>
            <Image src="EnemyAI.png"/>
            <p>Now when a single enemy can follow us, let's get super famous and get a whole group of stalkers.</p>
            <p>In order to make more enemies spawn and to give the monster a more natural hive-mind feel, we implemented a bunch of
                "nests" that are controlled by the enemey spawner script.
            </p>
            <Image src="Spawner.png"/>
            <p>So now with multiple stalkers coming at us, what is the most rational way to deal with them? </p>
            <p>Well, by having a massive futuristic gun of course!</p>
            <Image src="Gun.png"/>
            <p>In order to give the gun that realistic american feel, we mapped the input to the trigger of the controller. That gave it the feel of shooting a real gun.</p>
            <p>Handling the shooting functionality is done by applying force on the instantiated bullet, which reacts with the on triggerEnter of the "Destoryer" script,
                 therefore bringing annihilation to everything that stands in your path!</p>
                 <ol>
                     <li>
                         Shooting script
                         <Image src="Shoot.png"/>
                     </li>
                     <li>
                        Annihilation achiever
                        <Image src="death.png"/>

                     </li>
                 </ol>
                 <p>Implementing these functionalities concluded the week.</p>

</Text>
   
</Post>