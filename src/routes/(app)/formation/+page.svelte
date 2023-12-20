<svelte:head>
    <title>Formation & Hobbies</title>
</svelte:head>


<div class="text">
    <h1>Formation et Diplômes</h1>
    <div class="row">
            <span>&gt; 2022-2025 </span>
            <span class="pink">BUT Informatique </span>
            <span>IUT de Lille</span>
    </div>
    <div class="row">
        <span>&gt; 2022 </span>
        <span class="pink">Bac Général - Mention Très Bien Section Européenne </span>
        <span>Lycée Alexandre Ribot, Saint-Omer</span>
        <span>Spécialités Numérique et Sciences de l'Informatique (NSI) et Langues, Littérature et Civilisations Etrangères : Anglais (LLCE)</span>
    </div>
    <div class="row">
        <span>&gt; 2022 </span>
        <span class="pink">Anglais Certification Niveau B2+</span>
        <span>Certification Cambridge (204725119300003)</span>
    </div>

    <h1> Hobbies </h1>
    <span class="hobby">&gt; Dessin</span>
    <span class="hobby">&gt; Jeux Vidéo</span>
    <span class="hobby">&gt; Langues</span>
</div>
    
<style>
    span{
        font-size: 20px;
    }
    .row{
        display:flex;
        flex-direction: column;
        margin-bottom: 5px;
    }
        
    .text{
        display:flex;
        justify-content: center;
        flex-direction: column;
        width:50%;
        padding:75px 25px 0 25px;
    }

    .pink{
        text-decoration: inherit;
        color:#AB5650;
    }

    h1{
        font-family: "EastKind";
        font-weight: 200;
        color:#AB5650;
        font-size: 50px;
    }

    .hobby{
        margin-bottom: 15px;
    }
</style>