<svelte:head>
    <title>portfolio</title>
</svelte:head>

<div>
    <h1>port<br/>folio</h1>
    <form action="accueil">
        <input type="submit" value="Continuer" />
    </form>
    <p>Manon Leclercq | Etudiante en Informatique</p>
</div>

<style>
    h1{
        font-family: 'EastKind',sans-serif;
        color: #AB5650;
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

    input{
        background-color: #D4A7A0;
        border:0;
        border-radius: 33px;
        padding:10px 50px;

    }

    input:hover{
        background-color:#AB5650;
        
    }
</style>