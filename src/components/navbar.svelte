<script>
    import TranslateButton from "./translateButton.svelte";
</script>

<div id="navbarContainer">
		<div id="homeNav" class="nvlContainer"><a id="home" class="navLinks" href=".">Home</a></div>
		<div class="nvlContainer"><a class="navLinks" href="#about">About</a></div>
		<div class="nvlContainer"><a class="navLinks" href="#projects">Projects</a></div>
		<div class="nvlContainer"><a class="navLinks" href="#contact">Contact</a></div>
		<TranslateButton></TranslateButton>
</div>

<style>
	* {
		margin: 0;
		/* border: 1px solid red; */
	}


	@keyframes pop-in {
		from {
			scale: 0.75;
			opacity: 0;
		}

		to {
			scale: 1;
			opacity: 1;
		}
	}

	@keyframes fade-in {
		from {
			opacity: 0;
		}

		to {
			opacity: 1;
		}
	}

	::-webkit-scrollbar {
		width: 10px;
	}

	/* Track */
	::-webkit-scrollbar-track {
		background: #000;
	}

	/* Handle */
	::-webkit-scrollbar-thumb {
		background: #fff;
	}

	/* Handle on hover */
	::-webkit-scrollbar-thumb:hover {
		background: #555;
	}

	#navbarContainer {

		position: fixed;
        right: 0;
		top: 0;
		z-index: 10;
		width: 100%;
		height: 0vh;
		background-color: rgb(29, 29, 29);
		display: flex;
		flex-direction: column;
		align-items: flex-end;
		gap: 5%;

	}

	.navLinks {
		font-family: "Rajdhani";
		font-size: clamp(0.85rem, 1.5vw, 1.25rem);
		font-weight: 600;
		color: white;
		text-decoration: none;
		padding-right: 5%;
	}

	.nvlContainer {
		margin-right: 5%;
		margin-top: 0.5%;
		position: relative;
		width: fit-content;
		height: fit-content;
	}

	.nvlContainer::before {
		position: absolute;
		content: "";
		bottom: 0;
		left: 0;
		width: 0%;
		height: 2.5px;
		background-color: white;
		transition: 200ms;
	}

	.nvlContainer:hover::before {
		width: 100%;
	}

	#homeNav {
		margin-top: 2.5%;
	}
</style>