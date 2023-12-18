<svelte:head>
    <title>Compétences</title>
</svelte:head>


<div class="all">
    <div class="text">
        <h1>Compétences</h1>
        <div class="columns">
            <div class="firstColumn">
                <span>&gt; Java</span>
                <span>&gt; Python</span>
                <span>&gt; SQL</span>
                <span>&gt; Linux</span>
            </div>
            <div class="secondColumn">
                <span>&gt; HTML/CSS</span>
                <span>&gt; Svelte</span>
                <span>&gt; Photoshop</span>
                <span>&gt; Figma</span>
            </div>
        </div>
    </div>
    <div class="manuel">
        
    </div>
</div>
    
    <style>
        
    .all{
        display:flex;
        width:100%;
        box-sizing: border-box;
        padding:100px 25px 0 25px;
        justify-content: space-between;
    }
    
    .columns{
        display:flex;
        margin:20px;
    }
    
    .firstColumn,.secondColumn{
        display:flex;
        flex-direction: column;
        font-size: 25px;
        margin-right:50px;
    }
    
        
    
    .manuel{
        background-color: black;
        height:60vh;
        width:50%;
    }

    .columns span{
        margin-bottom: 25px;
    }

    .text{
        display:flex;
        justify-content: center;
        flex-direction: column;
        width:35%;
    }

    h1{
        font-family: "EastKind";
        font-weight: 200;
        color:#AB5650;
        font-size: 50px;
    }
</style>