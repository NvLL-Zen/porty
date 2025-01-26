<div class="nameContainer">
    <h1 class="name" id="leftName">
        FAUZAN
    </h1>
    
    <h1 class="name" id="rightName">
        RIZKY
    </h1>
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
</style>