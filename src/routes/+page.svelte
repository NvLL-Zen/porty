<script>
	import Section from "../components/section.svelte";
	import { onMount } from "svelte";
	const sleep = ms => new Promise(r => setTimeout(r, ms));

	onMount(() => {
		var c = document.getElementById("myCanvas");
		var ctx = c.getContext("2d");
		ctx.strokeStyle = "green"
		ctx.lineWidth = 5
		ctx.moveTo(0,250);

		function randomIntFromInterval(min, max) { // min and max included 
  		return Math.floor(Math.random() * (max - min + 1) + min);
		}

		let prevStonk;

		async function drawLines() {
			for(let i = 0; i < 500; i+= 10){
			
			
			let stonk = randomIntFromInterval(250 - i/2, 250 - i/3.25)
			
			if(i == 0) {
				prevStonk = stonk;
				console.log(`ini prevstonk ${prevStonk}`)
				console.log('ada')
			}
			
			
			ctx.lineTo(i,stonk);
			ctx.stroke();
			
			if(i > 0){
				console.log(prevStonk, stonk)
				if(prevStonk < stonk) {
				ctx.strokeStyle = "red"
				} else {
				ctx.strokeStyle = "blue"
				}
				await sleep(25);
				prevStonk = stonk
			} else {
				await sleep(25)
			}
			


			}
		}

		drawLines()
		
		

		
	})
</script>

<div class="mainApp">
	<Section>
		Hello im in section
	</Section>
	<Section>
		<canvas id="myCanvas" width="500" height="250" style="border:1px solid #d3d3d3;">
			Your browser does not support the HTML canvas tag.</canvas>
	</Section>
</div>


<style>
	.mainApp {
		width: 100vw;
		margin: 0;
		padding: 0;
		background-color: black;
		color: white;
		border: none;
	}
</style>