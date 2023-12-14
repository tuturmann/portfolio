
<svelte:head>
    <title>Présentation</title>
</svelte:head>

<div class="text">
    <h1>
        Bonjour !
    </h1>
    
    <img class="separator" src="line.png" alt="separator">

    <span>Je suis Manon, 19 ans, étudiante en deuxième année de BUT Informatique à Lille.</span>
    <span>Je recherche un stage en développement d’applications, développement web ou bases de données du <strong>15 avril au 21 juin 2024</strong>, avec si possible <strong>poursuite en alternance</strong>.</span>
</div>

<img class="drawing" src="home-portfolio.png" alt="background drawing">


<style>
    .text{
        margin: 15px;
        display:flex;
        justify-content: center;
        align-items: start;
        flex-direction: column;
        position:fixed;
        top: 60px;
        width:35%;
        
    }

    span{
        margin-top: 25px;
    }

    h1{
        font-family: "EastKind";
        font-weight: 200;
        color:#AB5650;
        font-size: 50px;
    }

    .drawing{
        float:right;
        
        height:100vh;
        z-index: -1;
    }
    .separator{
        width:75%;
    }

</style>