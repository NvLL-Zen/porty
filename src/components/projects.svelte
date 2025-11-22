<script>
    import nethackPic from "../images/nethack.png";
    import scefcoPic from "../images/scefco.png";
    import '../styles/anim.css'
    import { onMount } from 'svelte';

</script>

<div class="projectMain">
    <h1 id="projects">PROJECTS</h1>
    <div class="projectEntry left">
        <div class="projectImg">
            <a target="_blank" href="https://bit.ly/scefco"
                ><img class="popIn" src={scefcoPic} alt="scefco" /></a
            >
        </div>
        <div class="projectCaption">
            <h3 class="projectName">SCEFCO'24</h3>
            <p class="pop-in">
                A website that i voluntarily made for my school's annual
                competition event, it is used as a website to view information
                about the event, and to sign up for the competitions, aswell as
                view the terms & conditions of it. made w/ love :)
            </p>
            <p class="fade-in">Last Updated: December 2024</p>
            <p>Tech Stack: Astro JS - Cloudflare Pages</p>
        </div>
    </div>
    <div class="projectEntry right">
        <div class="projectImg">
            <a target="_blank" href="https://github.com/nvll-zen/-nethack"
                ><img src={nethackPic} alt="nethack" /></a
            >
        </div>
        <div class="projectCaption">
            <h3 class="projectName">NetHack</h3>
            <p>
                A program I made for network diagnostics and system information
                retrieval. This tool allows users to perform tasks like scanning
                Wi-Fi profiles, retrieving IP addresses, performing network
                pings, and locating IPs.
            </p>
            <p>Last Updated: March 2022</p>
            <p>Tech Stack: Python</p>
        </div>
    </div>
</div>

<style>
    :root {
        --projectHeight: 50vh;
        --projectMain_Height: 120vh;
    }
    * {
        color: white;
        font-family: "Rajdhani";
        /* border: 1px solid red; */
    }

    p {
        font-size: clamp(0.85rem, 1.1vw, 1.25rem);
        font-weight: 600;
    }

    .projectName {
        font-size: clamp(0.85rem, 1.25vw, 1.9rem);
    }

    .projectMain {
        width: 60vw;
        height: var(--projectMain_Height);
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        justify-content: space-between;
    }

    .projectEntry {
        display: flex;
        height: var(--projectHeight);
        width: 100%;
        gap: 2.5%;
    }

    .left {
        flex-direction: row;
    }

    .right {
        flex-direction: row-reverse;
    }

    .projectImg {
        width: 70%;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .projectCaption {
        width: 30%;
        height: 70%;
        display: flex;
        flex-direction: column;
        gap: 7.5%;
    }

    img {
        width: 100%;
        height: fit-content;
        border: 1px solid white;
        transition: 0.5s;
    }

    img:hover {
        scale: 1.05;
    }

    #projects {
        font-size: clamp(1.5rem, 10vw, 5rem);
    }

    @media only screen and (max-width: 720px) {
        :root {
        --projectHeight: 50vh;
        --projectMain_Height: 120vh;
        }
        .projectMain {
            width: 80vw;
        }
        .projectImg {
            width: 100%;
            height: 40%;
        }
        .projectCaption {
            width: 100%;
            height: 45%;
        }
        .projectEntry {
            gap: 5%;
        }
        img {
            width: 100%;
        }
        .left {
            flex-direction: column;
        }

        .right {
            flex-direction: column;
        }
    }
</style>
