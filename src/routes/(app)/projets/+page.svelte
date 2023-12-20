<script>
    import Cloud from "../../../components/Cloud.svelte";


    import Skill from "../../../components/Skill.svelte";

</script>
<svelte:head>
    <title>Projets</title>
</svelte:head>

<div class="body">

    <div class="title">
        
        <h1>
            Projets
        </h1>
        
        <span> Sur cette page, je répertorie tous mes projets en lien avec l'informatique.</span>
        
        <h2>Sommaire</h2>
        
        <div class="summarySection"><img src="flower.png" alt="flower icon"> <a href="#projet1">Deliver'Eat</a></div>
        <div class="summarySection"><img src="flower.png" alt="flower icon"> <a href="#projet2">Plateforme de covoiturage</a></div>
        <div class="summarySection"><img src="flower.png" alt="flower icon"> <a href="#projet3">Ilyva</a></div>
        <div class="summarySection"><img src="flower.png" alt="flower icon"> <a href="#projet4">Morpion</a></div>

    </div>
    
    <div id="projet1" class="projet">
        <Cloud name="01"/>
        <h2>Deliver'Eat</h2>
        <div class="competences">
            <Skill name="Java"/>
            <Skill name="Git"/>
        </div>

        <img class="illustration" src="delivereat.jpg" alt="delivereat projet agile">
        
        <img class="separator" src="line.png" alt="separator">
        
        <span>RPG joué dans le terminal qui possède un système de combat au tour par tour (bloquer, attaquer, utiliser un objet), d’inventaire, d’objets.</span>
        
        <span>Projet réalisé par groupe de 4 selon la méthode agile.</span>

        <a class="lienProjet" href="https://gitlab.univ-lille.fr/2023-projet-agile-de-rentree/groupe-13">Lien (il faut avoir un compte GitLab)</a>

        <span class="year">2023</span>
    </div>
    
    <div id="projet2" class="projet">
        <Cloud name="02"/>
        <h2>Plateforme de covoiturage</h2>
        <div class="competences">
            <Skill name="HTML/CSS"/>
            <Skill name="Figma"/>
            <Skill name="Wordpress"/>
        </div>
        
        <img class="illustration" src="plateformecovoiturage.png" alt="plateforme de covoiturage design figma">

        <img class="separator" src="line.png" alt="separator">
        
        <span>Plateforme de covoiturage en ligne réalisée sur Wordpress puis sur Figma, et enfin codée en HTML/CSS, où l'on devait respecter la charte graphique du site d'Ankama.</span>
        
        <span>Projet réalisé par groupe de 2.</span>
        <span class="year">2022</span>
    </div>
    
    <div id="projet3" class="projet">
        <Cloud name="03"/>
        <h2>Ilyva</h2>
        <div class="competences">
            <Skill name="Suivi de projet"/>
            <Skill name="Clip Studio Paint"/>
            <Skill name="Notion"/>
            <Skill name="Bash"/>
        </div>
        
        <img class="separator" src="line.png" alt="separator">
        
        <img class="illustration" src="ilyva.jpg" alt="plateforme de covoiturage design figma">

        <span>Escape game dans lequel l’objectif est de s’échapper d’un monde alternatif où Bash règne. Ce projet permet d’approfondir ses connaissances en Bash en jouant.</span>
        <span>J’ai réalisé tous les dessins ainsi que les énigmes en Bash.</span>
        <span>Projet réalisé par groupe de 5.</span>
        <a class="lienProjet" href="https://ilyva.sciencesky.fr">Lien pour jouer au jeu</a>
        <span class="year">2023</span>
    </div>

    <div id="projet4" class="projet">
        <Cloud name="04"/>
        <h2>Morpion</h2>
        <div class="competences">
            <Skill name="Bash"/>
        </div>
        
        <img class="separator" src="line.png" alt="separator">
        
        <img class="illustration" src="morpion.png" alt="plateforme de covoiturage design figma">

        <span>Morpion réalisé en Bash en autodidacte pour apprendre le langage.</span>
        <a class="lienProjet" href="https://github.com/tuturmann/tictactoe">Lien GitHub</a>
        <span class="year">2023</span>
    </div>
    
</div>
    
    <style>
    .lienProjet{
        font-size: 25px;
        text-decoration: underline wavy salmon 2px;
    }

    .illustration{
        position:absolute;
        object-fit: contain;
        width:25%;
        height:500px;
        transform:translateY(-50%);
        box-sizing: border-box;
        top:50%;
        left:50%;
    }

    .summarySection a{
        font-size: 35px;
    }

    span{
        font-size: 25px;
    }

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
        padding: 0 0 20px 0;
    }

    .projet{
        height:80vh;
        position: relative;
        display:flex;
        flex-direction: column;
        padding:50px 25px 50px 25px;
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
        font-size: 45px;
    }

    .title{
        display:flex;
        justify-content: center;
        flex-direction: column;
        width:50%;
        padding:75px 25px 0 25px;
    }

    .body {
        padding-bottom: 250px;
    }


</style>