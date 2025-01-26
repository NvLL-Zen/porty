<script>
	import Section from "../components/section.svelte";
	import Projects from "../components/projects.svelte";
	import Banner from "../components/banner.svelte";
	import About from "../components/about.svelte";
	import Name from "../components/name.svelte";
	import { onMount } from "svelte";
</script>

<div class="mainApp">
	<!-- <Navbar /> -->
	<Section>
		
		<Name></Name>
	</Section>
	<Banner></Banner>
	<Section>
		<About></About>
	</Section>
	<Section height=150>
		<Projects/>
	</Section>
</div>


<style>
	
	.mainApp {
		margin: 0;
		padding: 0;
		background-color: rgb(29, 29, 29);
		color: white;
		border: none;
		position: relative;
	}

	* {
		margin: 0;
		padding: 0;
		font-family: "Rajdhani";
		overflow-x: hidden;
	}
</style>