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
            Expérience professionnelle
        </h1>
        
        <span> Sur cette page, je répertorie mes expériences professionnelles.</span>
        
        <h2>Sommaire</h2>
        
        <div class="summarySection"><img src="flower.png" alt="flower icon"> <a href="#cgi">CGI</a></div>
    

    </div>
    
    <div id="cgi" class="projet">
        <Cloud name="01"/>
        <h2>CGI</h2>
        <div class="competences">
            <Skill name="PL/SQL"/>
            <Skill name="Oracle Data Integrator"/>
            <Skill name="Java"/>
            <Skill name="Git"/>
            <Skill name="SAP-BI"/>
            <Skill name="TIBCO BW"/>
            
        </div>
        
        <img class="separator" src="line.png" alt="separator">
        
        <span>J'ai eu la chance de travailler chez CGI pour un stage d'avril 2024 à juillet 2025. Par la suite, on m'a réembauchée en alternance pour mon année scolaire 2024-2025.</span>
        
        <span>Je travaille pour le client AG2R LA MONDIALE, pour qui nous développons et maintenons des fonctionnalités pour une application pour les gestionnaires.</span>

        <span>Nous développons cette application en Java et SQL principalement. J'ai eu la chance de travailler sur la réécriture des services qui étaient en Tibco BW vers Java.</span>

        <span>J'ai aussi repris la relève sur le travail d'un de mes collègues sur Oracle Data Integrator</span>

        <span class="year">2024-2025</span>
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
        height:20%;
        position: relative;
        display:flex;
        flex-direction: column;
        padding:50px 25px 50px 25px;
    }

    .projet span{
        width:35%;
        padding: 10px 0 10px 0;
        text-align: justify;
    }

    .competences{
        
        font-size: 20px;
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