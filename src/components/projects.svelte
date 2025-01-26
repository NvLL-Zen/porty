<div class="projectMain">
    <h1>PROJECTS</h1>
    <div class="projectEntry left">
        <div class="projectImg"></div>
        <div class="projectCaption">
            <h3 class="projectName">SCEFCO</h3>
            <p>
                A website that i voluntarily made for my school's annual
                competition event, it is used as a website to view information
                about the event, and to sign up for the competitions, 
                aswell as view the terms & conditions of it. made w/ love :)
            </p>
            <p>Last Updated: December 2024</p>
            <p>Tech Stack: Astro JS - Cloudflare Pages</p>
        </div>
    </div>
    <div class="projectEntry right">
        <div class="projectImg"></div>
        <div class="projectCaption">
            <h3 class="projectName">NetHack</h3>
            <p>
                A program I made for network diagnostics and system information
                retrieval. This tool allows users to perform tasks like scanning
                Wi-Fi profiles, retrieving IP addresses, performing network
                pings, and locating IPs.
            </p>
            <p>Last Updated: December 2024</p>
            <p>Tech Stack: Astro JS - Cloudflare Pages</p>
        </div>
    </div>
</div>

<style>
    * {
        color: white;
        font-family: "Rajdhani";
        border: 1px solid red;
    }

    .projectMain {
        width: 60vw;
        height: 150vh;
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        justify-content: space-between;
    }

    .projectEntry {
        display: flex;
        height: 50vh;
        width: 100%;
    }

    .left {
        flex-direction: row;
    }

    .right {
        flex-direction: row-reverse;
    }

    .projectImg {
        border: 1px solid rgb(0, 255, 0);
        width: 70%;
    }

    .projectCaption {
        width: 30%;
        height: 70%;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
    }
</style>
