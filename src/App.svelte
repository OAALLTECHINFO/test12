<style>
	@import url("https://unpkg.com/fluent-svelte/theme.css");
	:global(body) {
		background-color: var(--fds-solid-background-base);
		color: var(--fds-text-primary);
	}
</style>

<script>
	import { Router, Route, Link } from "svelte-navigator";
	import { TextBox , Button } from "fluent-svelte";
	import GradientText from 'svelte-gradient-typography';
	let value = "";
	import blog from "./blog.svelte";
</script>

<TextBox placeholder="Chose a Name" bind:value />

<Button href="/blog" >
	Blog
</Button>

<GradientText>
    The {value}
</GradientText>

<Button href="https://www.youtube.com/channel/UCHKlIYMRw7XhpVhGmysPKDA" variant ="accent" >
	Subscribe
</Button>
