<svelte:head>
    <title>Accueil</title>
</svelte:head>

<div class="parent">
    <img class="wallpaper" src="wallpaper.png" alt="landscape"/>
    <img class="montagnes" src="montagnes.png" alt="mountain on top of landscape"/>
    <div class="nuages">
        <img class="nuage1" src="nuage1.png" alt="cloud 1">
        <img class="nuage2" src="nuage2.png" alt="cloud 2">
    </div>
</div>
<div class="title">
    <h1>port<br/>folio</h1>
</div>

    
<style>

    .parent{
        position:fixed;
        z-index: -1;
        top:0;
        left:0;
        width:100%;
        height:100%;
    }

    .montagnes{
        z-index: 2;
        height:100vh;
        width:100%;
        position:fixed;
        overflow:hidden;
        top:0;
        left:0;
    }

    .wallpaper{
        height:100vh;
        width:100%;
        position:fixed;
        overflow:hidden;
        z-index: -1;
        user-select: none;
        top:0;
        left:0;
    }

    .nuages{
        width:100%;
    }

    .nuage1{
        z-index: 1;
        top:50%;
        position:absolute;
        height:200px;
        animation: slideshow 30s linear infinite;

    }

    .nuage2{
        top:20px;
        z-index: 0;
        height:200px;
        position:absolute;
        animation: slideshow 40s linear infinite reverse;
        
    }


    @keyframes slideshow {
        0% {
            left:-50%;
        }

        100% {
            left:100%;
        }
    }


    h1{
        font-family: "EastKind";
        color: black;
        font-size: 5em;
        letter-spacing: 1.5px;
        user-select: none;
    }
    
    .title{
        display:flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        height:100vh;
    }

</style>