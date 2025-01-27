<script>
    
    export let message = "COMPUTER SCIENCE • PORTOFOLIO • "
    export let direction = "left"
    
    let bannerMessage = message+message+message+message+message+message+message+message+message
    console.log(bannerMessage)
</script>
<div class="bannerContainer">
{#if direction === "left"}
<h3 class="mainBanner left">{bannerMessage}
</h3>
<h3 class="mainBanner left">{bannerMessage}
</h3>
{:else}
<h3 class="mainBanner right">{bannerMessage}
</h3>
<h3 class="mainBanner right">{bannerMessage}
</h3>
{/if}
</div>
<style>
    * {
        overflow-x: hidden;
    }

    .mainBanner {
        width: max-content;
        font-size: 1.5rem;
    }

    .left {
        animation: banner 10s linear;
        animation-iteration-count: infinite;
    }

    .right {
        transform: translateX(-100%);
        animation: bannerReverse 10s linear;
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

    @keyframes bannerReverse {
        to {
            transform: translateX(0%);
        }
    }
</style>
