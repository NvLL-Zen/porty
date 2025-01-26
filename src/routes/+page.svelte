<script>
	import Section from "../components/section.svelte";
	import Banner from "../components/banner.svelte";
	import About from "../components/about.svelte";
	import Name from "../components/name.svelte";
	import { onMount } from "svelte";
</script>

<div class="mainApp">
	<Section id="home">
		<Name></Name>
	</Section>
	<Banner></Banner>
	<Section>
		<About></About>
	</Section>
</div>


<style>
	.mainApp {
		margin: 0;
		padding: 0;
		background-color: black;
		color: white;
		border: none;
	}

	* {
		margin: 0;
		padding: 0;
		font-family: "Rajdhani";
		overflow-x: hidden;
	}
</style>