<svelte:head>
    <title>Accueil</title>
</svelte:head>

<img src="background-accueil.jpg" alt="landscape"/>
    <div>
        <h1>port<br/>folio</h1>
    </div>
    
    <style>
    img{
        background-image: url("background-accueil.jpg");
        height:100vh;
        width:100%;
        position:fixed;
        z-index: -1;
    }

    h1{
        font-family: "EastKind";
        color: black;
        font-size: 5em;
        letter-spacing: 1.5px;
        user-select: none;
    }
    
    div{
        display:flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        height:100vh;
    }

</style>