<script>
    import Cloud from "../../../components/Cloud.svelte";


    import Skill from "../../../components/Skill.svelte";

</script>
<svelte:head>
    <title>Projets</title>
</svelte:head>

<div class="title">

    <h1>
        Projets
    </h1>

    <span> Sur cette page, je répertorie tous mes projets en lien avec l'informatique.</span>
    
    <h2>Sommaire</h2>
    
    <div class="summarySection"><img src="flower.png" alt="flower icon"> <span>Deliver'Eat</span></div>
    <div class="summarySection"><img src="flower.png" alt="flower icon"> <span>Plateforme de covoiturage</span></div>
    <div class="summarySection"><img src="flower.png" alt="flower icon"> <span>Ilyva</span></div>
</div>

<div class="projet">
    <Cloud name="01"/>
    <h2>Deliver'Eat</h2>
    <div class="competences">
        <Skill name="Java"/>
        <Skill name="Git"/>
    </div>

    <img class="separator" src="line.png" alt="separator">

    <span>RPG joué dans le terminal qui possède un système de combat au tour par tour (bloquer, attaquer, utiliser un objet), d’inventaire, d’objets.</span>

    <span>Projet réalisé par groupe de 4 selon la méthode agile.</span>
    <span class="year">2023</span>
</div>

<div class="projet">
    <Cloud name="02"/>
    <h2>Plateforme de covoiturage</h2>
    <div class="competences">
        <Skill name="HTML/CSS"/>
        <Skill name="Figma"/>
        <Skill name="Wordpress"/>
    </div>

    <img class="separator" src="line.png" alt="separator">

    <span>Plateforme de covoiturage en ligne réalisée sur Wordpress puis sur Figma, et enfin codée en HTML/CSS.</span>

    <span>Projet réalisé par groupe de 2.</span>
    <span class="year">2022</span>
</div>

<div class="projet">
    <Cloud name="03"/>
    <h2>Ilyva</h2>
    <div class="competences">
        <Skill name="Suivi de projet"/>
        <Skill name="Clip Studio Paint"/>
        <Skill name="Notion"/>
        <Skill name="Bash"/>
    </div>

    <img class="separator" src="line.png" alt="separator">

    <span>Escape game dans lequel l’objectif est de s’échapper d’un monde alternatif où Bash règne. Ce projet permet d’approfondir ses connaissances en Bash en jouant.</span>
    <span>J’ai réalisé tous les dessins et les énigmes.</span>
    <span>Projet réalisé par groupe de 5.</span>
    <a href="https://ilyva.sciencesky.fr">Lien pour jouer au jeu</a>
    <span class="year">2023</span>
</div>

<style>
    .year{
        color:grey;
    }

    a{
        text-decoration: none;
        color:#AB5650;
    }

    .separator{
        width: 35%;
        height:1px;
        padding: 20px 0 20px 0;
    }

    .projet{
        height:80vh;   
        position: relative;
        display:flex;
        flex-direction: column;
    }

    .projet span{
        width:35%;
        padding: 10px 0 10px 0;
    }

    .competences{
        
        font-size: 30px;
        display: flex;
        flex-direction: column;
    }

    .projet{
        padding:0 25px 0 25px;
    }

    img{
        height:20px;
        width:20px;
    }

    h1{
        font-family: "EastKind";
        font-weight: 200;
        color:#AB5650;
        font-size: 50px;
    }
    h2{
        font-family: "EastKind";
        font-weight: 200;
        color:#AB5650;
        font-size: 35px;
    }

    .title{
        display:flex;
        justify-content: center;
        flex-direction: column;
        width:50%;
        padding:75px 25px 0 25px;
    }


</style>