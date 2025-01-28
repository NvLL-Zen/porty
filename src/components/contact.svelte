<script>
    import spotify from "../images/spotify.png";
    import github from '../images/github.png'
    import instagram from "../images/instagram.png";
    import email from "../images/email.png";
</script>

<div id="contact">
    <div class="contactMain">
        <h1 class="contactTitle">FIND ME HERE</h1>
        <div class="linkContainer">
            <div class="mobileHorizontal">
                <a target="_blank" href="mailto:v.zenriel@proton.me"
                ><img src={email} alt="" />v.zenriel@proton.me</a
            >
            <a
                target="_blank"
                href="https://github.com/nvll-zen"
                ><img src={github} alt="" />NvLL-Zen</a
            >
                <a target="_blank" href="https://instagram.com/fauzanrizky.n"
                ><img src={instagram} alt="" />fauzanrizky.n</a
            >
            <a
                target="_blank"
                href="https://open.spotify.com/user/31bepk3hehswxyz35dizjhpz6344"
                ><img src={spotify} alt="" />Zenriel V.</a
            > 
            </div>
            <div class="halfHorizontal">
                <a target="_blank" href="mailto:v.zenriel@proton.me"
                ><img src={email} alt="" />v.zenriel@proton.me</a
            >
            <a
                target="_blank"
                href="https://github.com/nvll-zen"
                ><img src={github} alt="" />NvLL-Zen</a
            >
            
            </div>
            <div class="halfHorizontal">
                <a target="_blank" href="https://instagram.com/fauzanrizky.n"
                ><img src={instagram} alt="" />fauzanrizky.n</a
            >
            <a
                target="_blank"
                href="https://open.spotify.com/user/31bepk3hehswxyz35dizjhpz6344"
                ><img src={spotify} alt="" />Zenriel V.</a
            >   
            </div>
            
        </div>
    </div>
</div>

<style>
    /* * {
        border: 1px solid red;
    } */

    a {
        color: white;
        text-decoration: none;
        font-size: clamp(0.85rem, 1.4vw, 1.6rem);
        font-weight: 700;
        
        padding: 2%;
        width: 90%;

        border: 1px solid white;
        border-radius: 10px;
        
        display: flex;
        flex-direction: row;
        justify-content:left;
        align-items: center;
        gap: 5%;
    }

    img {
        width: 20%;
    }

    @keyframes findmehere {
        0% {
            letter-spacing: 25px;
        }

        25% {
            letter-spacing: normal;
        }

        75% {
            letter-spacing: normal;
        }

        100% {
            letter-spacing: 25px;
        }
    }

    #contact {
        width: 100vw;
        height: 60vh;
        margin: 0;
        padding: 0;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .contactMain {
        width: 60%;
        height: 100%;
        display: flex;
        flex-direction: column;
        align-items: left;
        justify-content:space-between;
    }

    .contactTitle {
        height: 20%;
        font-size: clamp(1.5rem, 10vw, 5rem);
        animation: findmehere 3s ease-in-out infinite;
    }
    .linkContainer {
        display: flex;
        flex-direction: row;
        height: 72.5%;
        
    }
    .halfHorizontal {
        width: 35%;
        height: 100%;
        display: flex;
        flex-direction: column;
        gap: 7.5%;
    }

    .mobileHorizontal {
        display: none;
    }

    @media only screen and (max-width: 720px) {
        .contactMain {
            width: 80%;
            justify-content: flex-start;
        }

        .contactTitle {
            animation: none;
            height: 15%;
        }

        .linkContainer {
            height: 80%;
        }

        .halfHorizontal {
            display: none;
        }

        .mobileHorizontal {
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        
        }

        a {
            width: 90%;
            font-size: clamp(1.5rem, 2vw, 2.5rem);
        }
    }
</style>
