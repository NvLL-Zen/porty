<script>
    // import { writable } from "svelte/store";

    // const sleep = (ms) => new Promise((r) => setTimeout(r, ms));

    // function getRandomInt(min, max) {
    //     const minCeiled = Math.ceil(min);
    //     const maxFloored = Math.floor(max);
    //     return Math.floor(Math.random() * (maxFloored - minCeiled) + minCeiled); // The maximum is exclusive and the minimum is inclusive
    // }

    // let leftName = "FAUZAN";
    // let leftNameStr = writable(leftName);

    // let rightName = "RIZKY"
    // let rightNameStr = writable(rightName)

    // let holder = [];
    // let charInput = ''

    // let alphaNum = "ABCDEFGHIJLKMNOPQRSTUVWXYZ1234567890";
    // for (let i = 0; i < leftName.length; i++) {
    //     charInput = alphaNum[getRandomInt(0, alphaNum.length)]
    //     holder.push(charInput)
    // }

    // console.log(holder.join(''))

    // async function matrixText(delay, limitGuess, target, store) {
    // let holder = [];

    // for(let i = 0; i < target.length; i++) {
    //     let limit = 0
    //     while(holder[i] !== target[i]){
    //         limit += 1
    //         charInput = alphaNum[getRandomInt(0, alphaNum.length)]
    //         holder[i] = charInput
    //         console.log(holder.join(''))
    //         store.set(holder.join(''))
    //         await sleep(delay)
    //         if(holder[i] == target[i] || limit == limitGuess){
    //             holder[i] = target[i]
    //             store.set(holder.join(''))
    //             break
    //         } else {
    //             continue
    //         }
    //     }
    // }
    // }

    // matrixText(30, 3, leftName, leftNameStr);
    // matrixText(30, 3, rightName, rightNameStr);
</script>

<div id="home" class="nameContainer">
    <h1 class="name" id="leftName">
        FAUZAN
    </h1>
    <h1 class="name" id="rightName">RIZKY</h1>
</div>

<style>
    * {
        padding: 0;
        margin: 0;
        /* border: 1px solid red; */
    }

    .name {
        margin-left: -3%;
        padding-left: 3%;
        padding-right: 3%;
        position: relative;
        font-size: clamp(3rem, 10vw, 10rem);
        font-weight: 500;
        width: 60vw;

        animation: inspand 1s ease-out forwards;
    }

    @keyframes inspand {
        from {
            filter: brightness(0);
            width: 30vw;
        }

        to {
            filter: brightness(1);
            width: 60vw;
        }
    }

    #leftName::before {
        position: absolute;
        content: "";
        top: 0;
        left: 0;
        width: clamp(5px, 5vw, 50px);
        height: clamp(1px, 5vw, 10px);
        background-color: white;
    }

    #leftName::after {
        position: absolute;
        content: "";
        top: 0;
        left: 0;
        width: clamp(1px, 5vw, 10px);
        height: clamp(5px, 5vw, 50px);
        background-color: white;
    }

    #rightName::before {
        position: absolute;
        content: "";
        bottom: 0;
        right: 0;
        width: clamp(1px, 5vw, 10px);
        height: clamp(5px, 5vw, 50px);
        background-color: white;
    }

    #rightName::after {
        position: absolute;
        content: "";
        bottom: 0;
        right: 0;
        width: clamp(5px, 5vw, 50px);
        height: clamp(1px, 5vw, 10px);
        background-color: white;
    }

    #rightName {
        text-align: right;
    }

    @media only screen and (max-width: 720px) {
        #leftName::before,
        #leftName::after,
        #rightName::before,
        #rightName::after {
            width: 0;
            height: 0;
        }

        .name {
            width: 75vw;
            font-size: clamp(5rem, 10vw, 10rem);
        }
    }
</style>
