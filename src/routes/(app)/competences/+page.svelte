<script lang="ts">

    const skills = [
        {
            name: "java",
            description: "Java est un langage orienté-objet. En BUT Informatique à Lille, nous utilisons principalement Java pour développer des applications. La plupart de mes projets est en Java."
        },
        {
            name: "python",
            description: "Python est un langage de programmation que j'ai appris au lycée. Il permet de faire de l'orienté-objet, il possède une large communauté qui apporte de multiples librairies et API. J'ai par exemple utilisé l'API de Discord pour faire un bot. Je l'ai aussi"
        },
        {
            name: "sql",
            description: "SQL est un langage qui permet de communiquer avec une base de données. J'ai utilisé PostgreSQL à l'IUT et PL/SQL à CGI."
        },
        {
            name:"noSQL",
            description: "Durant ma formation, j'ai appris à utiliser des langages de type noSQL tels que MongoDB, Cassandra, Redis"
        },
        {
            name: "linux",
            description: "Linux est un système d'exploitation open-source. J'ai des compétences en BASH, un shell répandu en Linux, j'ai notamment réalisé un <a href=\"projets#projet4\"> morpion </a> dans ce langage."
        },
        {
            name: "html/css",
            description: "HTML/CSS est un langage de style permettant de réaliser des site web en front-end."
        },
        {
            name:"javascript/typescript",
            description: "Javascript est un langage que j'ai notamment utilisé pour du front-end, en Svelte et React principalement mais aussi sans framework pour mon projet BreakingKart."
        },
        {
            name: "svelte",
            description: "Svelte est un framework liant html, css et javascript. Ce portfolio est codé en Svelte."
        },
        {
            name:"react",
            description: "React est un framework liant html, css et javascript. Je l'ai utilisé durant ma formation à l'IUT."
        },
        {
            name: "photoshop",
            description: "Photoshop est un logiciel d'édition d'images. Je l'utilise pour dessiner, ainsi que d'autres logiciels concurrents tels que ClipPaint Studio."
        },
        {
            name: "figma",
            description: "Figma est un site web permettant de faire des maquettes de sites web. Je l'ai notamment utilisé pour faire ce portfolio, mais aussi pour tous mes autres projets web."
        },
        {
            name:"spring",
            description: "Spring est un framework Java qui permet de définir l'infrastructure d'un projet. Je l'ai utilisé à CGI et à l'IUT."
        },
        {
            name:"odi",
            description: "Oracle Data Integrator est une plate-forme d'intégration de données pour hauts volumes. Je l'ai utilisé à CGI pour la maintenance des sauvegardes des données."
        }
    ];

    let index = -1;

</script>

<svelte:head>
    <title>Compétences</title>
</svelte:head>

<div class="all">
    <div class="text">
        <h1>Compétences</h1>
        <div class="columns">
            <div class="separateColumn">
                <button on:click={() => index = 0}>&gt; Java</button>
                <button on:click={() => index = 1}>&gt; Python</button>
                <button on:click={() => index = 2}>&gt; SQL</button>
                <button on:click={() => index = 3}>&gt; NoSQL</button>
            </div>
            <div class="separateColumn">
                <button on:click={() => index = 5}>&gt; HTML/CSS</button>
                <button on:click={() => index = 6}>&gt; Javascript & Typescript</button>
                <button on:click={() => index = 7}>&gt; Svelte</button>
                <button on:click={() => index = 8}>&gt; React</button>
                <button on:click={() => index = 12}>&gt; Oracle Data Integrator</button>
            </div>
            <div class="separateColumn">
                <button on:click={() => index = 11}>&gt; Spring</button>
                <button on:click={() => index = 4}>&gt; Linux</button>
                <button on:click={() => index = 9}>&gt; Photoshop</button>
                <button on:click={() => index = 10}>&gt; Figma</button>
            </div>
        </div>
    </div>

    <div class="manuel">
        {#if index === -1}
            <p>Cliquez sur une compétence pour voir le texte</p>
        {:else}
            <span>manon@portfolio:~$ man {skills[index].name}</span>
            <p>{@html skills[index].description}</p>
        {/if}
    </div>
</div>
    
<style>
    .manuel :global(a){
        color:white;
    }

    .manuel :global(a:visited){
        color:white;
    }

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
    
    .columns button{
        text-decoration: underline;
        border:none;
        background: none;
        margin-bottom: 25px;
        font-size: 30px;
        cursor:
        url(/hk.png) , auto;
    }

    
    .separateColumn{
        display:flex;
        flex-direction: column;
        font-size: 25px;
        margin-right:50px;
        white-space: nowrap;
    }

    .manuel{
        background-color: black;
        height:60vh;
        width:40%;
        color: white;
        padding: 10px;
        box-sizing: border-box;
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