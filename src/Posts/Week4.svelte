<script>
    import Post from "../Post.svelte";
    import Title from "../Title.svelte";
    import Text from "../Text.svelte";
</script>

<Post>
    <Title>Markerless Week 1 - Setting up the project</Title>
    <Text>
        Experimenting with AR Markerless.<br/>
        Outlining the plan for our app and brainstorming.<br/>
        Museum like experience<br/>
        Users can place and walk around sights<br/>
    </Text>
    <Text>
        For the first weeek of working with markerless AR we were just trying to set everything up, see how it works and plan our 
        project accordingly.
    </Text>
    <Text>
        We had a brainstorming session in which we came up with 3 ideas and then voted on which one we will implement. In the end, it was decided that we will try to 
        provide a museum like experience and make it so you could look at various monuments around the world and learn a little bit about them. 
    </Text>
    <Text>
        It was a bit tricky to get it working as the markerless AR needed to correctly scan the planes and selecting the items was also an issue. When we figured it out we 
        made the project as if you were next to the actual monument and could inspect it in detail while learning interesting facts about the structure. We settled to 
        implement the Statue of Liberty and The Eiffel Tower.
    </Text>
    <Text>
        This was implemented by setting two smaller models of the monuments and allowing the user to select which one he wants to place and then inspect. After you place the object
         you can click the monument and see different facts about it allowing you to learn more about it.
    </Text>
    
</Post>
