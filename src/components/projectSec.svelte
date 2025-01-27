

<div class="sectionProject">
    <slot>
    
    </slot>
</div>

<style>
    .sectionProject {
        height: 150vh;
    
        margin: 0;
        padding: 0;
        /* border: 1px solid red; */
        
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        z-index: 1;
    }

    @media only screen and (max-width: 720px) {
        .sectionProject {
            height: 130vh;
        }
    }
</style>