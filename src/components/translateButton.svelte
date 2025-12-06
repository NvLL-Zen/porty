<script>
    import { onMount } from "svelte";
    let currentLang = "EN"; 

    // 2. Define reactive variables to manage the styles directly
    let ENBg = "white";
    let ZHBg = "black";

    // 3. Function to toggle the language and update styles
    function toggleLanguage() {
        if (currentLang === "EN") {
            currentLang = "ZH";
            ENBg = "black";
            ZHBg = "white";
        } else {
            currentLang = "EN";
            ENBg = "white";
            ZHBg = "black";
        }
    }
    
</script>


<button id="translateButton" on:click={toggleLanguage}>
    <h6 id="ENSign" style:background={ENBg} style:color={ZHBg}>EN</h6>
    <h6 id="ZHSign" style:background={ZHBg} style:color={ENBg}>ZH</h6>
</button>


<style>
    * {
        border: 1px solid white;
        transition: all 0.25s ease-out;
    }
    #translateButton {
        scale: 1.1;
        font-family: "Rajdhani";
		font-size: clamp(0.85rem, 1.5vw, 1.25rem);
		font-weight: 600;
		text-decoration: none;
        color: white;
        background-color: black;
        display: flex;
        flex-direction: row;
        justify-content: center;
        padding: 0;
        transform: translateX(-20%);

        margin-right: 5%;
		margin-top: 0.5%;
		position: relative;
		width: fit-content;
		height: fit-content;
    }

    h6 {
        font-size: clamp(0.85rem, 1.5vw, 1.25rem);
        width: 150%;
        
    }

    #ENSign {
        padding-right: 5%;
        padding-left: 5%;
    }

    #ZHSign {
        padding-right: 5%;
        padding-left: 5%;
    }
</style>
