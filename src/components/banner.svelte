<script>
    import { onMount } from "svelte";
    
    
</script>

<div class="bannerContainer">
<h3 id="mainBanner">COMPUTER SCIENCE • PORTOFOLIO • COMPUTER SCIENCE • PORTOFOLIO • COMPUTER SCIENCE • PORTOFOLIO • COMPUTER SCIENCE • PORTOFOLIO • COMPUTER SCIENCE • PORTOFOLIO • COMPUTER SCIENCE •
</h3>
<h3 id="mainBanner">COMPUTER SCIENCE • PORTOFOLIO • COMPUTER SCIENCE • PORTOFOLIO • COMPUTER SCIENCE • PORTOFOLIO • COMPUTER SCIENCE • PORTOFOLIO • COMPUTER SCIENCE • PORTOFOLIO • COMPUTER SCIENCE •
</h3>


</div>
<style>
    * {
        overflow-x: hidden;
    }

    h3 {
        width: max-content;
        font-size: 1.5rem;
        animation: banner 5s linear;
        animation-iteration-count: infinite;
    }

    .bannerContainer {
        transform: translateY(-5vh);
        display: flex;
        width: fit-content;
        gap: 0;
        padding-top: 1px;
        padding-bottom: 1px;
        border: 0.5px solid white;
    }

    @keyframes banner {
        to {
            transform: translateX(-100%);
        }
    }
</style>