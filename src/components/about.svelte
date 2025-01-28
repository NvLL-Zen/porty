
<h1 id="about" class="aboutSign">
    WHO AM I?
</h1>
<div class="aboutMain">
    <div class="aboutHalf" id="aboutHalfLeft">
        <h3 class="jobTitle">(Future) Software Engineer</h3>
        <div class="aboutNav">
            <div>
                <h3 class="NavDesc">
                    Web Development
                </h3>
                <h3 class="NavDesc">
                    Data Science
                </h3>
            </div>
            <div>
                <h3 class="NavDesc"><a target="_blank" href="https://github.com/nvll-zen">Github ↗</a></h3>
            </div>
        </div>
    </div>
    <div class="aboutHalf" id="aboutHalfRight">
        <h3 class="aboutDesc">
            Self taught CS student with an experienced knowledge of Python, and Javascript. 
            I am passionate about computers and technology since i was little, intriguing my curious mind.
        </h3>
        <h3 class="aboutDesc">
            Currently i'm a highschool student in Indonesia, still developing and sharpening my skills. Trying to balance
            between life and my hobby, aswell as preparing into college
        </h3>
        <h3 class="aboutDesc">I am fluent in both Bahasa Indonesia and English, i'm also learning Japanese</h3>
        <h3 class="aboutDesc">
            Feel free to reach out to me and say hello :)
        </h3>
    </div>
</div>

<style>

    /* * {
        border: 1px solid red;
    } */

    a {
        color: white;
        text-decoration: none;
    }

    .aboutSign {
        font-size: clamp(1.5rem, 10vw, 5rem);
        font-weight: 900;
        padding-bottom: 1%;
        width: 60vw;
        line-height: 100%;
        height: min-content;
        animation: blinking 1.5s linear infinite;
    }

    .aboutMain {
        width: 60vw;
        height: 50vh;
        display: flex;
        flex-direction: row;
        color: rgb(230, 230, 230);
    }

    .aboutHalf {
        width: 50%;
        height: 100%;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
    }

    #aboutHalfRight {
        justify-content: space-between;
    }

    .aboutDesc {
        font-weight: 600;
        font-size: clamp(0.85rem, 1.25vw, 1.75rem);
    }

    .aboutNav {
        width: 100%;
        align-self: flex-end;
        justify-self: flex-end;
        box-sizing: border-box;
        padding: 1%;

        display: flex;
        flex-direction: row;
        gap: 5%;

        font-weight: 500;
    }

    .NavDesc {
        font-size: clamp(0.85rem, 1.25vw, 1.9rem);
    }

    .jobTitle {
        box-sizing: border-box;
        padding: 1%;
        font-size: clamp(1.5rem, 2.5vw, 5rem);
        text-shadow: 0px 0px 4px white;
        font-weight: 700;
    }

    @media only screen and (max-width: 720px){
        .aboutSign {
            width: 80vw;
        }

        .aboutMain {
            width: 80vw;
            height: 75vh;
            flex-direction: column;
            justify-content: space-between;
        }

        .aboutHalf {
            width: 100%;
            height: 50%;
        }

        #aboutHalfLeft {
            height: 20%;
        }

        #aboutHalfRight {
            height: 50%;
        }

        .jobTitle {
            font-size: clamp(1.5rem, 2vw, 3rem);
        }

        .aboutDesc {
            font-size: clamp(1rem, 1.5vw, 1.5rem);
        }

        #aboutHalfRight {
            align-self: flex-end;
        }


    }

    @keyframes blinking {
        0% {
            opacity: 1;
        }

        50%  {
            opacity: 0;
        }

        100% {
            opacity: 1;
        }
    }


</style>