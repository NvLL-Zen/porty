<script>
	import Section from "../components/section.svelte";
	import ProjectSec from "../components/projectSec.svelte";
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
	<ProjectSec>
		<Projects/>
	</ProjectSec>
	<Banner direction="right" message="SAY HI SAY HI SAY HI "></Banner>
</div>


<style>
	:root {
		--mobile: false;
	}
	
	.mainApp {
		margin: 0;
		padding: 0;
		background-color: black;
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

	@media only screen and (max-width: 720px){
		:root {
		--mobile: true;
		}
	}
</style>