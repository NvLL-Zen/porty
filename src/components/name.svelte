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
        margin-left: -2.5%;
        padding-left: 2.5%;
        padding-right: 2.5%;
        position: relative;
        font-size: 10rem;
        font-weight: 500;
        width: 60vw;
    }

    #leftName::before {
        position: absolute;
        content: "";
        top: 0;
        left: 0;
        width: 50px;
        height: 10px;
        background-color: white;
    }

    #leftName::after {
        position: absolute;
        content: "";
        top: 0;
        left: 0;
        width: 10px;
        height: 50px;
        background-color: white;
    }

    #rightName::before {
        position: absolute;
        content: "";
        bottom: 0;
        right: 0;
        width: 10px;
        height: 50px;
        background-color: white;
    }

    #rightName::after {
        position: absolute;
        content: "";
        bottom: 0;
        right: 0;
        width: 50px;
        height: 10px;
        background-color: white;
    }

    #rightName {
        text-align: right;
    }
</style>