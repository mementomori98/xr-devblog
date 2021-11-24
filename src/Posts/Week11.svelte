<script>
    import Post from "../Post.svelte";
    import Title from "../Title.svelte";
    import Text from "../Text.svelte";
    import Image from "../Image.svelte";
</script>

<Post>
    <Title>XR Project Week 2 "How to Spiderman?"</Title>
   <Text>
       <p>During this week the primary objective of the group was to get a skeleton up and running.</p>
       <p>We decided that the most important feature of this game was a fluent swinging mechanic. Hence, we set to implement that</p>
        
       <p>And so our journey began, first of all we should metion that our swinging mechaninc was greatly inspired by the tutorial from
           Denis Tutorials which you could check out it <a href="https://youtube.com/watch?v=Xgh4v1w5DxU&feature=share"
           >here! </a>
       </p>
       <h3>The challenge!</h3>
       <p>The primary challenge was to craete the script in VR so that the experience feels smooth. The approach we took was by attaching an anchor to the "ceiling" whilst having a "SpringJoint" attached to the XR rig.
           The spring joint is created or destroyed each time the player pushesh or releases the trigger on the controller. We should also mention that the shooting of the web is 
           dependant on the raycast, hence if the raycast doesn't hit anything, the procedure is not executed. Ones an object has been hit, a rope is drawn from the tip of the XR Rig to the grappleable object that is the "ceiling".
           Furthermore, there a few other things the script includes, such as:
           
       </p>
       <ol>
        <li>
            A maximum distance, tracking whether the player is too far away to shoot a web
        </li>
        <li>
            Pulling speed, that manages lenghtening or shorthening the lenght of the rope whilst it is attached to the "ceiling".

        </li>
    </ol>
       <p> With this our week was concluded and our childhood dream of being a superhero was one step closer to becoming a reality...a virtual one to be exact.</p>
       <Image src="spinderman.png"/>
   </Text>

   
</Post>