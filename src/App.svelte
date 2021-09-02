<script>
	import Post from "./Post.svelte";
	import Title from "./Title.svelte";
	import Code from "./Code.svelte";
	import Tab from "./Tab.svelte";
	import Image from "./Image.svelte";
	import Text from "./Text.svelte";
</script>

<div class="layout">
	<div class="appbar">

	</div>
	<div class="content">
		<Post>
			<Title>Post 1</Title>
			<Text>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aliquid cupiditate delectus deserunt ea earum enim eos fuga id iusto mollitia odit praesentium quam qui, quis quod recusandae sunt unde voluptas?</Text>
			<Code>
				public static void main()<br/>
					<Tab/>Hello
			</Code>
		</Post>
		<Post>
			<Title>Post 2</Title>
			<Text>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusamus amet delectus doloribus ducimus ea est, id, incidunt, iste laborum nesciunt nihil perspiciatis quaerat quia quo rem reprehenderit rerum sapiente. Totam?</Text>
			<Text>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusamus amet delectus doloribus ducimus ea est, id, incidunt, iste laborum nesciunt nihil perspiciatis quaerat quia quo rem reprehenderit rerum sapiente. Totam?</Text>
			<Image src="https://media.wired.com/photos/598e35fb99d76447c4eb1f28/master/pass/phonepicutres-TA.jpg"/>
			<Text>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusamus amet delectus doloribus ducimus ea est, id, incidunt, iste laborum nesciunt nihil perspiciatis quaerat quia quo rem reprehenderit rerum sapiente. Totam?</Text>
		</Post>
		<Post>
			<Title>Post 3</Title>
			<Text>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Architecto ducimus enim eveniet explicabo fuga id neque nesciunt nostrum, quaerat quasi quidem quod repellendus voluptas. Beatae deserunt magnam optio perferendis praesentium.</Text>
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