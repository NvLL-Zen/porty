<script>
    export let height = 100;
</script>

<div class="section" style="height: {height}vh;">
    <slot>
    
    </slot>
</div>

<style>
    .section {
    
        margin: 0;
        padding: 0;
        /* border: 1px solid red; */
        
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }
</style>